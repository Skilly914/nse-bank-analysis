# NSE Bank Analysis

A comparative financial analysis of seven Kenyan banks listed on the Nairobi Securities Exchange (NSE), covering profitability, efficiency, liquidity, and asset quality over 2021–2025. Built with Excel and Power BI.

Overview page

Objectives
The project answers five questions:

1. Profitability: Which banks earn the most, and how consistently?
2. Efficiency: Which banks run the leanest cost base?
3. Liquidity: What does holding more liquidity cost in profit?
4. Shocks: How did the 2022–2023 rate and exchange-rate pressures show up in the ratios?
5. Scale: Does bank size predict performance?

Banks covered;
KCB Group, Co-operative Bank of Kenya, NCBA Group, Absa Bank Kenya, I&M Group, Standard Chartered Bank Kenya and Diamond Trust Bank Kenya. 

I excluded Equity Group Holdings because I could not consistently source all required fields from its audited statements. As a result, totals in this project cover seven banks, not the whole listed sector.

Key findings;
- Profit more than doubled. Combined profit after tax of the seven banks rose from about KES 84bn in 2021 to about KES 187bn in 2025. 
- Profit is concentrated. KCB earned KES 233bn of the KES 700bn total over 2021–2025 (33%). With Co-operative Bank (KES 117bn), the top two account for half of all profit.
- No bank leads on every measure. Absa leads on average ROE (24.6%) and runs a lean cost base, but lends about 91% of its deposits. Standard Chartered Kenya pairs strong returns with the most cautious balance sheet (loan-to-deposit about 49%).
- Size does not predict returns. Mid-sized banks rank first and second on ROE, the largest bank (KCB) ranks third, and Diamond Trust Bank ranks last.
- Efficiency does not explain returns. Diamond Trust Bank has the lowest cost-to-income ratio (about 39%) but the lowest ROA (1.4%) because its margin is thin.
- Lending and liquidity trade-off. Banks that lend more of their deposits hold less liquidity, but all stay well above the 20% statutory minimum.
- Loan quality is weak across the sector. Average NPL ratios range from about 10% to 16%, with KCB highest. 
- Provisions peaked in 2023. Combined loan loss provisions rose to about KES 79bn in 2023 before easing, with KCB accounting for 43–47% of the total in 2023–2025.
- Standard Chartered Kenya is the 2025 exception. Its profit fell 38% to KES 12.4bn while the other six banks grew profit.

Dashboard pages
1. Overview	- Profit after tax by bank and by year, with headline KPIs
2. Profitability	- ROE, ROA and net interest margin by year, plus profit growth
3. Efficiency and liquidity -	Cost-to-income, loan-to-deposit, and lending against liquidity
4. Asset quality -	NPL ratio, liquid assets ratio and loan loss provisions
5. Peer comparison -	One matrix ranking all banks across the key ratios

Profitability, efficiency, and liquidity, Asset quality, Peer comparison

Data and method

Sources: audited consolidated financial statements and official results announcements published by each bank (via the banks' investor relations pages. 

Verification. The first version of the dataset came from a mix of sources with inconsistent definitions. Every figure was re-checked against audited or officially published results. Checks included:

> Net interest income = interest income less interest expense
> Total operating income less expenses and provisions = profit before tax
> Total assets = total liabilities + equity
> Calculated ratios compared with bank-reported ratios

Where a bank's full audited statements were unavailable, figures from its official results announcement were used. 

Units and basis: KES millions, consolidated (Group) figures, as reported. 2020 is used only to provide opening balances for average-based ratios, so the analysis window is 2021–2025.

Ratio definitions
- ROE	- Profit after tax ÷ average of opening and closing total shareholders' equity
- ROA -	Profit after tax ÷ average of opening and closing total assets
- Net interest margin	Bank-reported - (interest-earning assets are not consistently disclosed)
- Cost-to-income	- Total operating expenses (excluding loan loss provisions) ÷ total operating income
- Loan-to-deposit -	Net loans and advances ÷ customer deposits
- Statutory liquidity ratio	Bank-reported, the CBK regulatory measure (minimum 20%)
- Liquid assets ratio	- (Government securities + cash and CBK balances) ÷ total assets
- NPL ratio -	Gross non-performing loans ÷ gross loans and advances

Shareholders' equity excludes non-controlling interest, applied the same way for every bank. Because the cost-to-income ratio here excludes provisions, it can differ from each bank's own published figure.

Repository structure
nse-bank-analysis/
├── README.md
├── dashboard/
│   ├── nse_bank_analysis.pbix
│   └── nse_bank_analysis.pdf
├── data/
│   ├── NSE_bank_analysis.xlsx
│   └── audited company results
└── images/
    └── 01_overview.png 
    └── 02_profitability.png 
    └── 03_liquidity.png 
    └── 04_asset_quality.png 
    └── 05_peer_comparison.png 
    
How to use
Download dashboard/nse_bank_analysis.pbix.
Open it in Power BI Desktop, which is free and runs on Windows.
I have also uploaded the Excel file I used to collect the data.
A PDF export and screenshots are provided for anyone without Power BI.

Limitations;
- Seven banks, not the whole sector. Equity Group is excluded, so totals and averages do not describe the listed market.
- Small sample. With seven banks, differences between tiers and rankings are patterns to explore, not statistical proof.
- Averages are unweighted. Peer averages treat each bank-year equally and are not weighted by size.
- Five-year averages hide trends. Rankings on the peer comparison page average 2021–2025, so a single strong year (for example, Standard Chartered Kenya in 2024) can lift a bank's position.
- Definitions differ across banks. Provisions, liquid assets, and NPL definitions are not identical in every bank's disclosures.
- Context is not causation. Links to the 2022–2023 interest rate and exchange rate environment are offered as context, not as something this data proves.

Tools;
Microsoft Excel (data model and checks), Power Query and DAX (Power BI).

Author;
Clinton Muriuiki 
https://www.linkedin.com/in/clinton-muriuki-/

Disclaimer
This project is for learning and portfolio purposes. It is not investment advice.
