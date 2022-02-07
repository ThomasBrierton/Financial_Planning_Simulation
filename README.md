# Financial_Planning_Simulation

This is a financial planning tool used to help client's plan for retirement. The tool runs a monte carlo with the client's portfolio values, potential weighting options, and a retirement timeline of 10 and 30 years. The tool estimates performance and potential outcomes.

---

## Technologies 

This project uses Jupyter Notebook (within JupyterLab) and the standard Python 3.8 libraries. In addition, this project requires the following libraries and/or dependencies:

- Pandas - a software library designed for open source data analysis and manipulation

- matplotlib - a cross-platform, data visualization and graphical plotting library for Python and its numerical extension NumPy

- os - provides a portable way of using operating system dependent functionality

- requests - allows you to send HTTP/1.1 requests easily. 

- json - JSON is a lightweight data format used for data interchange between multiple different languages.

- dotenv - reads key-value pairs from a .env file and can set them as environment variables

- alpaca_trade_api - a python library for the Alpaca Commission Free Trading API. 

- MCForecastTools - the document named "MCForecastTools.py" contains the code functions needed to run the Monte Carlo Simulations (MCSimulation) used in this project

- All stock and bond data was pulled in using Alpaca API calls to the Alpaca SDK. The ETH and BTC data were pulled in using the Requests library from the following links: btc_url, eth_url

---

## Methods

In order to use this financial planning tool, the following steps were performed:

Step 1: Collect the data of the portolio's holdings and gather the current prices using Alpaca API.

Step 2: Calculate the portfolio's value in USD.

Step 3: Plot a pie chart of the portolio.

Step 4: Calculate an emrguncy fund value based off the client's income.

Step 5: Run a monte carlo simulation over 30 years, with the portfolio weighted 60% stocks and 40% bonds. Plot the results, and obtain summary statistics. 

Step 6: Perform another monte carlo simulation over 10 years with the portfolio weighted 80% stocks and 20% bonds.

*To follow along and see more in-depth comments, please review the financial_planning_simulation.ipynb Jupyter Notebook file.

---

## Analysis

The financial planning tool produced useful results in helping the client determine if retirement in 10 years is a possibiliy. The portfolio weighted heavier towards stocks produced a range of return between $102,191.81 and $973,812.63 with 95% confidence. This is a good return, but other factors need to be taken into consideration to determine if the client is able to retire in 10 years. On the low end of the range, retirement would be very difficult. Knowing the client's lifestyle, health benefits, assets etc would be helpful to determine if the 10 year simulation would be realistic for retirement. Based off the initial findings, I would advize against retiring in 10 years. 

The 30 year simulation weighted 60% stocks and 40% bonds produced better returns, ranging from $523,310.27 and $9,337,080.01 with 95% confidence. These returns would set the client up better for retirement, especially since the length of retirement would be 20 years shorter. I would recommend the client to keep investing and working towards a larger retirement fund, one more in line with the 30 year simulation.

---

## Contributors

Thomas Brierton and UCB

---

## License

MIT