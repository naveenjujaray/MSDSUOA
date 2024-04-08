# Finance-And-Risk-Analytics

## Problem Statement:

The wealth management industry has grown significantly, leading to the emergence of portfolio managers who help individuals and businesses make investment decisions. Portfolio managers work with analysts to create suitable investment portfolios. However, they face competition and must use available resources effectively. In a case scenario, you're tasked with providing investment consultation to two investors, Mr. Patrick Jyenger and Mr. Peter Jyenger, based on their unique financial objectives.

## Solution Approach: 

The following is a summary of the key steps and processes involved in solving this problem:

### * Data Gathering:
To address the challenge, we initially gathered data on 24 different stocks from four different sectors, as well as data from the S&P 500.

### * Data Preprocessing:
Python was used to clean the dataset, removing any discrepancies and ensuring it was in a suitable format for analysis.

### * Data Visualization:
We leveraged the preprocessed data to generate Power BI reports for each sector. These reports allowed us to visualize and compare the performance of different stocks within each sector.

### * Metric Calculation:
Using Python, we calculated various metrics such as average daily return, average risk, annualized risk, annualized return, cumulative return, and Sharpe ratio. These metrics formed the basis for our investment decision-making process.

### * Portfolio Selection:
Based on the calculated metrics and careful analysis, we handpicked stocks that aligned with the specific financial objectives of Mr. Patrick Jyenger and Mr. Peter Jyenger. This resulted in the creation of tailored investment portfolios designed to meet their needs.

### * Presentation:
Finally, we created a comprehensive presentation that showcases all our findings and the rationale behind our stock selections. This presentation serves as a transparent and informative resource for our clients.

Please refer to the relevant sections and files in this repository for more details on each step of the project.
Problem Statement - I

It is recommended that you cover the basics of finance and risk analytics theory along with the Time Series Forecasting - I session, or you may keep going through that as and how you reach that part of the problem statement.

Let’s hear from Joydeep as he introduces the required elements here.
3052186

Let’s move the case at hand.
Business Case

In the recent past, the industry of wealth management has seen a lot of growth. Individuals and businesses actively seek maximum returns. However, in many cases, they lack either the skills to identify the right investment opportunities or the time to find such opportunities. This challenge gave rise to the dedicated individuals who perform this task on behalf of the investors for a commission: portfolio managers.

 A portfolio manager makes investment decisions and carries out other related activities on behalf of vested investors. They work with a team of analysts and researchers, and their main objective is to realize the needs of the investor and suggest a suitable portfolio that meets all the expectations. They are responsible for establishing the best investment strategy and selecting appropriate investments with the right allocations. However, in doing so, they face a lot of competition in the form of other portfolio managers and rival firms. Therefore, the portfolio manager has to use the available resources to provide the best solution to the investor.

 Consider yourself working for an associate at an investment firm that manages accounts for private clients. Your role requires you to analyze a portfolio of stocks to provide consultation on investment management based on client requirements. Let us hear more about it from Joydeep as he introduces you to the entire case.
3052186

Your task is to provide consultation to two different investors, Mr. Patrick Jyenger and Mr. Peter Jyenger based on their requirements and financial objectives. You can refer to the elements mentioned in the video to develop the investor persona. The image below summarizes the profile of the two investors:

 

You must perform the required steps for both the individuals after understanding the investor persona independently. But before, let’s hear about your tasks in more detail from Joydeep.
3052186

Following points summarise the expected tasks in the assignment:

    You must use the elements of technical analysis to understand the trend of the underlying stocks. The metrics associated with risk and returns must help you realise whether the security meets the criteria of your investor’s financial goals.
    You must use the metrics and the visualisations to compare the performance of the available securities against each other, and also against the market index, S&P500.
    The findings should be aligned with the investor persona to select the appropriate stocks for the portfolio.
    After the selection of stocks, the portfolio must be validated using the active investment strategy to estimate the prices in future. You must check if the portfolio has the potential to fulfil the financial goals set by the investor.

The next segment will help you with each task in detail. 

 
Data Description

You can download the data from the provided link below.
Dataset_Finance_DA_Capstone
Download

    You are provided with the following information for 24 stocks of leading companies listed in New York Stock Exchange(NYSE):
        Date
        Open price: Price of stock at the start of the day
        Close price: Price of stock at the end of the day
        High price: Highest price reached by the stock on that day
        Low price: Lowest price reached by the stock on that day
        Adjusted close price: Stock price adjusted to include the annual returns (dividends) that the company offers to the shareholders
        Volume traded: Number of stocks traded on the day
    The information for every stock ranges from 1st October 2010 to 30th September 2020.
    The stocks belong to different domains:
        Technology/IT
        Travel/Aviation/Hospitality
        Banking/Financial Services and Insurance
        Pharmaceuticals/Healthcare/Life Sciences
    To help you with the market benchmark, you are given the S&P 500 index prices for the same period.

 

Now, you have a good understanding of the data and the problem statement. The next segment will help you with the details of the expected tasks.

Problem Statement - II

After developing an understanding of the problem statement and the data set, it is important to think about your approach to solving the problem. The previous segment helped you with the broad overview of the steps, but now you will hear about each task in detail. The entire capstone can be divided into the following aspects:

    Preliminary Steps - Data loading
    Data Exploration
    Stock Analysis and Portfolio Management and Reporting the insights

 

Let’s hear from Joydeep about every element in detail:
3052186
Tasks 1: Preliminary Steps

Under preliminary steps, you are expected to load the entire data into the working environment (Python). The entire data must be merged into a single dataframe with only the required columns. Most importantly, you must ensure that you can identify the company and the industry from the collated data for company-specific and industry analysis.
Task 2: Data Exploration

As part of the exploration, you must create interactive visualization dashboards and evaluate the performance metrics that help summarize the stock. Here, you can use any visualization tool like Tableau, Python, etc. However, the final outcome should reflect all the points mentioned in the video. Moreover, the findings should be backed by your understanding of the concept or facts from the industry.
Task 3: Stock Analysis and Portfolio Management

As part of this task, you must execute your responsibilities as the portfolio manager. You must use the information about the investor to create a profile and use it along with the obtained results to create a portfolio of stocks that have the potential to meet the financial goals of both investors.

 

Hint: As part of the active investment strategy, try to replicate the daily gains/returns from the past five years over the future to predict the value of the selected stocks.

 

 Submissions Required

You will need to submit the following documents for this capstone project:

    A clean version of the final data set.
    A well-commented Jupyter notebook containing the entire work.

A file containing a dashboard or simply all visualizations that convey the insights asked in the project.