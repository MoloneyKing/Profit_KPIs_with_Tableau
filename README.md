# Profit_KPIs_with_Tableau
Project Proposal: Data Visualization for Sales
Performance Analysis
Using Super Store Dataset
Michelle Moloney King
Project Proposal: Data Visualization for Sales Performance Analysis by www.MichelleMoloneyKing.com
Project Proposal: Data Visualization for Sales Performance Analysis 3
Executive Summary: 3
Why: 3
Specific Outcomes: 3
Persona Documents: Persona 1: Sales Manager 4
Persona 2: Marketing Director 4
Dataset Description: 5
Reason for Dataset Selection: 5
Initial Opinion on Presenting Findings: 5
Foreseeable Challenges: 5
Determining Sales KPI 6
Profit Ratio 6
Profitability Ratio 6
Sales Spotlight 7
Lower Bond 8
Upper Bond 8
2
Project Proposal: Data Visualization for Sales Performance Analysis by www.MichelleMoloneyKing.com
Project Proposal: Data Visualization for Sales
Performance Analysis
See the tableau Public Data Visualisation on my profile.
Executive Summary:
The proposed project aims to create a data visualisation solution for analysing sales performance in a retail
organisation. The visualisation will provide insights into key sales metrics, identify trends, and help make
data-driven decisions. By leveraging data visualisation techniques, the project aims to enhance
understanding, improve sales performance, and optimise business strategies.
Why:
The objective of this project is to address the need for effective sales performance analysis in the retail
organisation. By visualising sales data, the project aims to provide actionable insights to improve sales
strategies, identify underperforming areas, and maximise revenue. The project will help stakeholders gain a
comprehensive understanding of sales patterns and make informed decisions to drive growth.
Specific Outcomes:
1. Visualise sales performance metrics, including revenue, units sold, and profit margins, to identify
trends and patterns.
2. Analyse the impact of external factors (e.g., marketing campaigns, seasonality) on sales
performance.
3. Identify top-performing products, regions, and sales representatives.
4. Provide interactive features for filtering and drill-down capabilities to explore data at different levels
of granularity.
3
Project Proposal: Data Visualization for Sales Performance Analysis by www.MichelleMoloneyKing.com
Persona Documents: Persona 1: Sales Manager
● Name: Alex Thompson
● Age: 40
● Gender: Male
● Photo: Physical description - Thompson is a 40-year-old male with a professional appearance. He
has a well-groomed, short brown hair that is neatly styled. His clean-shaven face highlights his sharp
jawline and emphasises a sense of professionalism. Alex has a fair complexion with a hint of tan,
indicating a moderate amount of outdoor activity.
● Goals: To identify areas of improvement in sales performance, track the effectiveness of sales
strategies, and make data-driven decisions to optimise sales operations.
● Challenges and Needs: Needs a clear overview of sales performance, actionable insights, and the
ability to drill down into specific regions or product categories for further analysis.
● Context: Will view the visualisation on a desktop computer or tablet during team meetings or while
analysing sales reports.
Persona 2: Marketing Director
● Name: Sarah Johnson
● Age: 35
● Gender: Female
● Photo: Johnson has short blond hair, neatly cut, she is wearing a sharp blazer, she has a dark
complexion.
● Goals: To understand the impact of marketing campaigns on sales, identify successful campaigns,
and allocate resources effectively for future marketing initiatives.
● Challenges and Needs: Requires an overview of sales performance in relation to marketing efforts,
the ability to filter data by campaign parameters, and the ability to compare different marketing
strategies.
● Context: Will interact with the visualisation on a large display during marketing strategy meetings
and campaign reviews.
4
Project Proposal: Data Visualization for Sales Performance Analysis by www.MichelleMoloneyKing.com
Dataset Description:
The chosen dataset for this project is a comprehensive sales dataset containing information such as
transaction dates, product details, sales representative information, region, revenue, and profit. The dataset
is available in CSV format and satisfies the criteria of having clean dates, relevant sales metrics, and no
problematic outliers.
Reason for Dataset Selection:
The selected dataset was chosen because it provides a rich set of sales data that encompasses various
aspects necessary for comprehensive analysis. It includes historical sales records and attributes that are
crucial for evaluating performance at different levels (e.g., product, region, time). By utilising this dataset, the
visualisation will offer valuable insights into sales performance and help stakeholders identify patterns,
trends, and areas for improvement.
Initial Opinion on Presenting Findings:
The findings will be presented through an interactive data visualisation dashboard using Tableau. The
dashboard will include various charts, graphs, and filters to provide an intuitive and exploratory user
experience. It will allow users to interact with the data, filter by different dimensions, and drill down to
specific details for deeper analysis. The visualisations will be designed to effectively communicate key sales
metrics, trends, and comparisons to facilitate decision-making.
Foreseeable Challenges:
1. Data Integration: Ensuring seamless integration of the sales dataset with Tableau and addressing
any data quality issues or inconsistencies.
2. Visualisation Design: Creating visually appealing and intuitive charts and graphs that effectively
convey information without overwhelming the users.
3. Data Security: Ensuring appropriate data privacy and security measures when sharing the
visualisation publicly on Tableau
5
Project Proposal: Data Visualization for Sales Performance Analysis by www.MichelleMoloneyKing.com
Determining Sales KPI
To do this I created a new category field with the elbow formula.
IF SUM([Sales]) >= 125000 then "Above Benchmark" ELSE "Below benchmark" END
Profit Ratio
Create a calculated field
SUM([Profit])/SUM([Sales])
Profitability Ratio
This was created from Profit Ratio.
IF ([Profit Ratio]) >= 0.33 THEN "GREAT" ELSEIF [Profit Ratio] > 0.1 THEN "OK" ELSE "BAD"
END
6
Project Proposal: Data Visualization for Sales Performance Analysis by www.MichelleMoloneyKing.com
Sales Spotlight
I broke this down by category and order date with a calculated field for sales spotlight
IF sum([Sales]) > 10000 then "Good" ELSE "Bad" END
7
Project Proposal: Data Visualization for Sales Performance Analysis by www.MichelleMoloneyKing.com
Lower Bond
New calculation field
WINDOW_AVG(SUM([Profit])) - (WINDOW_STDEV(SUM([Profit])) * [Std Dev])
Upper Bond
New calculation field
WINDOW_AVG(SUM([Profit])) +(WINDOW_STDEV(SUM([Profit]) * [Std Dev]))
8
Project Proposal: Data Visualization for Sales Performance Analysis by www.MichelleMoloneyKing.com
9
