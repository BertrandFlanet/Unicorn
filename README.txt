Step 1: Project Title and Description
Step 2: Table of Contents
Step 4: Usage
Step 5: Project Structure Describe the structure of your project directory. This helps readers understand where to find different components of your project.
Step 6: Data
Step 7: Analysis
Step 8: Results
Step 9: Visualizations
Step 10: Conclusions
Step 11: Contact



Unicorn is a family business owned by 2 stakeholders who are very invested in their business.<br>
The company focuses on e-commerce, trusting the common idea that the online sector has been slowly eating up market share in the past two decades. <br>
Unicorn's platform allows people to buy products online: from books, toys, clothes, and shoes to food, furniture, and other household items.<br>
<br>
We have been asked to analyze Unicorn's data, find interesting insights, and identify weak areas and opportunities for Unicorn to boost its business growth.
<br>
From our EDA, performed using SQL, and visualization produced in Tableau, we uncovered a key point of contention: a negative profit/discount correlation.
Our project dives into this finding and offers a possible solution to the issue.


- Table of Contents
1 - Introduction
2 - Table of Contents
3 - Usage
4 - Project Structure
5 - Data
6 - Analysis
7 - Results
8 - Visualisations
9 - Conclusions
10 - Acknowledgement
11 - Contact

- Usage
.ipynb: Google Colab: Upload directly via the "File" menu or open from Google Drive
Jupyter Notebook: Install Jupyter, start it via terminal, and open the .ipynb file through the interface

.twb: Open with Tableau - Tableau Public installation - https://public.tableau.com/

. If using another IDE, you will need the following libraries:
- pandas
- sqlalchemy
- psycopg2

- Project Structure
data/: Reference to dataset and used aggregated dataset at various granularity level
notebooks/: Jupyter notebooks with the analysis/segmentation code
results/: Output files, results, project report, .ppt presentation
README.md: Project documentation


- data

For security reasons, the database link cannot be directly shared.
Connection to the database is share through an .ini file using a sparse method.
Refer to the 'usage' section to read on its use.

Here is the structure of the database's tables and columns:
- customers
customer_id
customer_name
customer_segment
- order_details
order_details_id
order_id
product_id
quantity
order_discount
order_profits
order_profit_ratio
order_sales
- orders
order_id
customer_id
order_date
shipping_city
shipping_state
shipping_region
shipping_country
shipping_postal_code
shipping_date
shipping_mode
- product
product_id
product_name
product_category
product_subcategory
product_manufacturer


Alternatively, we provided a .csv document that contains all the database features within one single table to be found within the data repertory.


- Analysis
The analysis was conducted in the following three steps:
- Cleaning
- EDA using SQL
- Visualisation in Tableau


- Results
Through EDA, we investigated Unicorn data at multiple levels of granularity - State, city, product category, and product.
We observed that at each level the deficit in the revenue of Unicorn company could be tied to discounts offered to their customers.
Thus we concluded the existence of a negative correlation profit/discount.
Considering this observation, we also noted that the proposed discount average, no matter the financial status of the state, has remained the same from 2015 to 2018.
While it is sensical for states that generate profit to keep on applying a method that works, it is concerning that the same method has been applied with consistency for states in deficit.
This makes us wonder on why this issue hasn't been noticed and addressed earlier.


- Visualizations
Charts and plots are available in the following folder: results
The dashboard can be accessed with the following link: https://public.tableau.com/app/profile/bertrand.flanet/viz/Unicorn_viz/DashboardUnicorn2?publish=yes

- Conclusions
Despite the clear existence of the found negative correlation, we cannot assert with certainty that it is the main cause of Unicorn's underperformance.
For instance, it is noteworthy that despite deficits, certain cities have exhibited positive sales. Therefore, further exploration into the potential role of discounts in facilitating these sales, as well as an examination of factors that enhance their effectiveness is required. This may include evaluating the duration of discount eligibility and considering the socio-economic and demographic profiles of the targeted populations.

Meanwhile, we have provided a hands-on solution to urgently answer Unicorn dramatic deficits at various levels. Our dashboard displays the necessary discounts that should be offered at state, city, product category, and product levels to generate profits and re-establish a positive balance in the categories at a loss.

- Acknowledgement
This project has been conducted within the frame of Masterschool Data Analytics boot camp.
It was conducted as a duo composed of Bertrand Flanet and Nadyia Zahn

- Contact
Bertrand Flanet<br>
E-mail: bertrand.flanet@gmail.com<br>
linkedIn: https://www.linkedin.com/in/bertrand-flanet-67b1b2299/<br>

