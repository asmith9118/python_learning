# python_learning
Setup: 

        notepad $PROFILE for powershell settings that preloaded the mushrooms conda environment:
            conda activate ./mushrooms
            Remove-Item alias:r

        setting up conda environment:
            conda create --prefix C:\Users\Anthony\mushrooms python R numpy sympy pandas scikit-learn tensorflow matplotlib seaborn requests beautifulsoup4 jupyter r-essentials

        pip install rpy2[full]

        Python kernel:
            pip install ipykernel
            python -m ipykernel install --user --name mypythonkernel --display-name "Python (mypythonkernel)"

        Open any R session (e.g. in RStudio is fine, or open terminal/bash and type R to start an R session).
        Install the kernel with:
            install.packages("devtools")
            devtools::install_github("IRkernel/IRkernel")
            IRkernel::installspec()

        jupyter kernelspec list

        rpy kernel:
            kernel.json
                {
                "display_name": "rpy",
                "language": "python",
                "argv": [
                    "python",
                    "-m",
                    "ipykernel_launcher",
                    "-f",
                    "{connection_file}"
                ],
                "env": {
                    "R_HOME": "C:/Users/Anthony/mushrooms/Lib/R" 
                }
                }


Current notepad $PROFILE:
# Ensure fnm is available before running
if (Get-Command fnm -ErrorAction SilentlyContinue) {
    fnm env | Invoke-Expression
}

# Conda initialization workaround
$condaHook = "C:\Users\Anthony\miniconda3\shell\condabin\conda-hook.ps1"
$condaExe = "C:\Users\Anthony\miniconda3\condabin\conda.bat"

if (Test-Path $condaHook) {
    & $condaHook
    conda activate C:\Users\Anthony\mushrooms
} elseif (Test-Path $condaExe) {
    & $condaExe "shell.powershell" "hook" | Out-String | Invoke-Expression
    conda activate C:\Users\Anthony\mushrooms
} else {
    Write-Host "WARNING: Conda not found!"
}
