# python_learning

Week 1: 
    5/4/2024: 
        Installed python, VSCode, Git on devices - synced (win/macOS)
         Installed minicondas (win/macOS) and homebrew (macOS) 
        Python Data Science Handbook: Read up to chapter on Numpy

    5/9/2024:
        Climbed, hiked 8.0 miles
        Finished first chapter on numpy arrays
        Stay motivated, your work remains unfinished 

    5/12/2024:
        Chapter 6: Computation on Numpy Arrays: Universal Functions
        Activities: Climbed, played guitar, sang read Goggins, talked to mom and dad, walked cats, yoga, journal, 
        Utilized ChatGPT for defining a learning program 
        Utilized ChatGPT for learning python: debuging, defining funtions

    5/19/2024: 
        deep dive into kernels, set up rpy2 and have a kernel with the setting below saved in .json file
        
        overall I'm very happy with the progression today,
        continued to use chatGPT for help and it has been a lifesaver :

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
    5/20/24:
        Started lecture series on linear algebra: https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/download/ - I looked at the problem sets and they give me anxiety because I don't understand the language. I understand programming though, and I am pleased with my knowledge of matrixes. 

        Created numpy_cheatsheet, tried to use ChatGPT to format into colors but ran out of space

        Walked the cats, played a little bit of guitar, watched nuggets lose unforuntately, 40m yoga, bought weed, read goggins, signed up for meal kit service. Created goals for tomorrow. Stay motivated and attack the day. Go to sleep in the black. I want to read more  books about military leadership and training, I think. 

Phase 1: Python Proficiency (1-3 months)
    Weeks 1-4: Python Basics Refresher

        Review Python basics such as syntax, variables, data types, and control structures.
        Refresh your knowledge of functions, modules, and libraries in Python.
        Utilize resources like "Python Crash Course" by Eric Matthes or online tutorials for quick refreshers.
    
    Weeks 5-8: Data Manipulation in Python

        Dive into data manipulation using Python libraries like NumPy and pandas.
        Explore advanced data structures and techniques for efficient data handling and analysis.
        Practice applying your programming skills to real-world datasets relevant to finance and trading.
    
    Weeks 9-12: Advanced Python Topics

        Deepen your understanding of advanced Python concepts:
        Object-oriented programming (classes, inheritance, polymorphism)
        File handling, input/output operations, and exception handling.
        Explore Python libraries commonly used in finance and trading, such as Matplotlib for data visualization.

Phase 2: Finance and Trading Concepts (2-4 months)
    Weeks 13-16: Introduction to Finance

        Refresh your understanding of finance basics, focusing on concepts relevant to trading:
        Types of financial markets, asset classes, and investment vehicles.
        Key financial metrics and ratios used in fundamental analysis.
    
    Weeks 17-20: Technical Analysis and Market Dynamics

        Explore technical analysis techniques used in trading, building on your existing knowledge:
        Chart patterns, trend analysis, and support/resistance levels.
        Advanced technical indicators and oscillators.
        Analyze historical price data and identify trading signals using Python.
    
    Weeks 21-24: Algorithmic Trading Fundamentals

        Gain a solid understanding of algorithmic trading concepts and strategies:
        Market data collection and preprocessing.
        Strategy formulation, backtesting, and optimization.
        Risk management principles and position sizing strategies.

Phase 3: Implementation and Practice (3-6 months)
    Weeks 25-28: Backtesting and Strategy Development

        Implement trading strategies in Python, leveraging libraries like Backtrader or QuantConnect.
        Perform rigorous backtesting to evaluate strategy performance and refine your approach.
        Explore different optimization techniques to improve strategy profitability and robustness.

    Weeks 29-32: Automation and Integration

        Learn how to automate trading strategies using Python scripts or platforms like MetaTrader or Interactive Brokers.
        Integrate your algorithms with brokerage APIs for live trading execution.
        Implement risk management protocols and monitoring systems for automated trading.

    Weeks 33-36: Continuous Improvement and Adaptation

        Continuously monitor and analyze the performance of your trading strategies.
        Stay updated with developments in financial markets and algorithmic trading techniques.
        Iterate on your strategies, incorporating new insights and adapting to changing market conditions.
        Continuous Learning and Practice
        Dedicate time each week for reviewing concepts, exploring advanced topics, and working on personal projects.
        Stay engaged with the programming and trading communities through forums, online communities, and networking events.
        Consider participating in online courses, workshops, or webinars to deepen your knowledge and expand your skill set.
   