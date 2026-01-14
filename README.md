# blinkit-clone-Power-bi-dashboard

blinkit Sales Analysis – Power BI Dashboard (Clone Project)
!! Disclaimer
This project is a clone / practice-based analytical case study and does NOT use real Blinkit business data.
The dataset used is publicly available / simulated and the brand name “Blinkit” is used only for educational and learning purposes to demonstrate Power BI skills, data modeling, DAX calculations, and dashboard design.
This analysis does not represent actual Blinkit sales, performance, or internal business insights.
---------------------------------------------------------------------------------------------------
# Project Overview
This project is a Power BI dashboard clone created to simulate how a quick-commerce company (such as Blinkit) could analyze sales performance, customer behavior, and outlet efficiency within a specific geographic area.
The goal is to extract meaningful insights for a selected area using industry-relevant KPIs, interactive visuals, and DAX measures—similar to real-world business intelligence workflows.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Business Objectives
- Simulate sales performance analysis** for a quick-commerce business
- Analyze customer preferences** (fat content & item type)
- Compare outlet performance** by size, location, and type
- Identify area-level trends** and patterns
- Demonstrate end-to-end Power BI project execution**

---------------------------------------------------
# Tools & Technologies
- Excel (Data Source)
- Power BI Desktop
- DAX (Data Analysis Expressions)
- Power Query (Data Cleaning & Transformation)

-------------------------------------------------
## Dataset Description and Sorce 
The dataset is synthetic / practice-based and includes:

Item details

Outlet information

Sales values

Customer ratings

Outlet size, location & type

Source-https://drive.google.com/drive/folders/1mKh61zKVBnPJN0A5lc77osGNkmNa-loI(got from youtube )

---------------------------------------------------------------------------------------------------

#KPIs Created
KPI      	          Description
Total Sales	        Total revenue generated
Average Sales	      Average sales per item
Number of Items	    Total count of items sold
Average Rating	    Average customer rating
------------------------------------------------

## dax measured  used 
-- Total Sales
Total Sales = SUM('Blinkit'[Sales])

-- Average Sales
Average Sales = AVERAGE('Blinkit'[Sales])

-- Number of Items
Number of Items = COUNT('Blinkit'[Item Identifier])

-- Average Rating
Average Rating = AVERAGE('Blinkit'[Rating])
-----------------------------------------------------
#Advanced Analytical Measures
-- Sales Contribution %
Sales Contribution % =
DIVIDE(
    [Total Sales],
    CALCULATE([Total Sales], ALL('Blinkit'))
)

-- Total Sales by Outlet Type
Total Sales by Outlet Type =
CALCULATE(
    [Total Sales],
    ALLEXCEPT('Blinkit', 'Blinkit'[Outlet Type])
)

-- Average Sales by Outlet Size
Avg Sales by Outlet Size =
CALCULATE(
    [Average Sales],
    ALLEXCEPT('Blinkit', 'Blinkit'[Outlet Size])
)

------------------------------------------------------

## Dashboard Visuals & Purpose
Visual	                           Insight
KPI Cards	                    Overall performance snapshot
Donut Chart                 	Sales distribution by fat content
Bar Chart	                    Item-wise sales comparison
Line Chart                   	Sales trend by outlet establishment year
Donut Chart                 	Sales by outlet size
Bar Chart                   	Sales by outlet location
Matrix Table                	KPI comparison by outlet type
Slicers	                      Area-wise and outlet-wise filtering
-----------------------------------------------------------------------

## Dashboard Features
Interactive filter panel

Clear all slicers functionality (bookmark-based)

Sidebar navigation (mobile-inspired UI)

Consistent branding & layout design
-------------------------------------
## Key Insights 
Regular fat products contribute higher simulated sales

Tier 3 outlets outperform Tier 1 & Tier 2 in this sample area

Supermarket Type 1 shows higher revenue contribution

Medium-sized outlets show balanced performance
-----------------------------------------------
##Conclusion
This clone project demonstrates how Power BI can be used to:

Analyze sales data at an area level

Evaluate outlet and product performance

Support data-driven decision-making

Build professional, business-ready dashboards
-------------------------------------------------
## screenshot of Dashboard
link-https://github.com/shubhank7379/Blinkit-clone-Power-bi-dashboard/blob/main/blinkit%20dashboard%20img.png
