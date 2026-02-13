# Power BI Sales Dashboard

## Overview
This report analyzes sales performance by region and product.

## Files
- Medical Analysis Dashboard.pbip – Main report
- Hospital_Pharmacy_PowerBI.xlsx – Sample dataset

## How to Use
1. Download the .pbix file
2. Open in Power BI Desktop
3. Update data source if needed
4. Refresh

## Core Measures (DAX Layer)
### Core KPIs
1. Total Visits = DISTINCTCOUNT(Visits[Visit ID])
2. Total Pharmacy Revenue = SUM(Pharmacy[Total Cost])
3. Avg Length of Stay = AVERAGE(Visits[Length of stay days])

### Supporting Measures
1. Total Quantity = SUM(Pharmacy[Quantity])
2. Revenue per Visit = DIVIDE([Total Pharmacy Revenue], [Total Visits])

## Key Analytical Insights
### 1. Disease Distribution Across Counties

The matrix analysis reveals clear geographical variation in disease prevalence, indicating that disease burden is not uniformly distributed across counties.  

From a decision-making perspective, this insight supports county-level resource allocation, where high-prevalence counties should receive proportionally higher clinical capacity, diagnostic equipment, and pharmaceutical supply. 

### 2. Patient Visits vs Pharmacy Revenue

The positive correlation between total visits and total pharmacy revenue indicates that, in general, higher patient turnout drives higher pharmaceutical income. However, the relationship is not strictly linear, implying that not all visits contribute equally to revenue. 

Uasin Gishu emerging as the highest revenue-generating county suggests either higher patient volumes, more complex cases, or prescription of higher-cost medications. 

This highlights that revenue optimization is not only a function of volume but also of department mix and treatment intensity. This insight can inform pricing strategies, inventory planning, and identification of high-value service locations.

### 3. Departmental Cost Drivers

The pie chart analysis shows that the inpatient department accounts for the highest proportion of pharmacy costs (34.41%), slightly exceeding emergency and outpatient services. 

This aligns with clinical expectations, as inpatient care typically involves more complex treatment regimens, longer medication courses, and higher-cost drugs. 

This identifies inpatient services as the primary cost center for pharmaceutical expenditure, making it the most critical area for cost-control initiatives such as bulk purchasing and further investment.

### 4. Age-Based Medication Consumption

The age group analysis demonstrates a monotonic increase in medication usage with advancing age. 

This reflects the epidemiological reality that older populations experience higher disease burden and chronic conditions requiring sustained pharmacological management. 

This insight has strong strategic implications: the hospital should anticipate growing pharmaceutical demand as the patient population ages, particularly for chronic disease medications. It also supports proactive planning for geriatric care services, long-term treatment programs, and inventory forecasting focused on age-sensitive drug categories.

### 5. Length of Stay vs Revenue Efficiency

The combined analysis of average length of stay and revenue per visit highlights an important operational paradox. Conditions such as malaria and diabetes generate higher revenue per visit despite shorter hospital stays, whereas pneumonia, hypertension, and flu result in longer stays but lower revenue per visit. 

This indicates that some diagnoses are resource-intensive without being financially efficient, consuming bed capacity and clinical time without proportional revenue return. 

For hospital management, this insight is critical for capacity planning and service line evaluation. It suggests the need to redesign clinical pathways for long-stay, low-revenue conditions, potentially through outpatient management, preventive care, or improved discharge protocols to reduce inefficiencies.

## Overall Strategic Implication

Collectively, these insights show that hospital performance is driven not merely by patient volume, but by the interaction between disease mix, demographic structure, departmental workflows, and treatment economics. The dashboard enables management to identify where clinical demand is highest, where costs are concentrated, and where operational inefficiencies exist. This creates a foundation for evidence-based decisions in staffing, budgeting, pharmaceutical procurement, and long-term healthcare planning.
