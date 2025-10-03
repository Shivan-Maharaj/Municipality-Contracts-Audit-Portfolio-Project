# Municipal Contracts Audit Portfolio Project
## Project Background

This project was designed to audit municipal contracts to detect potential corruption, overspending, and compliance failures. Using Excel, Python, and Power BI, the goal was to classify contracts as Good or Bad, identify high-risk vendors and departments, and create an interactive dashboard for executives to visualize contract performance and financial exposure.

The dashboard addresses the following core questions:

How many contracts are flagged as Good vs Bad?

Which vendors contribute most to overspending?

How does actual spend compare to approved budgets?

What operational red flags exist across contracts?

How can contract management and vendor oversight be improved?

## Data Structure & Initial Checks

Analysis was based on a single unified dataset with 500 contracts, including the following fields:

• contract_id – Unique identifier for each contract.

• department – Responsible municipal department.

• vendor – Contracted vendor.

• approved_budget – Budgeted contract value.

• contract_value – Actual contract spend.

• deviation_flag – Indicates budget deviation.

• mbd_submitted – Missing or submitted MBD documentation.

• project_phase – Current phase of the project.

• status – Completion status.

• risk_score – Calculated risk for each contract.

• irregular_flag – Indicates irregular expenditure.

• irregular_amount – Value of irregular expenditure.

Preprocessing included: Standardizing numeric fields, validating contract IDs, labeling contracts as Good or Bad, and preparing measures for visualization in Power BI.

<img width="940" height="627" alt="Dashboard Screenshot Placeholder" src="ADD_YOUR_IMAGE_HERE" />

## Executive Summary

• 500 contracts were analyzed:
  
  • 185 (37%) were clean (Good).
  
  • 315 (63%) were flagged as Bad due to missing MBD documents, overspending, delays, or premature completion.

<img src="Project%202%20-%20Municipality%20Risk%20Assessment/Images/Good_vs_Bad_Donut.PNG" width="400">


**Financial overview:**

• Budgeted: R12.60 bn

  • Actual Spend: R13.21 bn

  • Overspend: R1.19 bn

**Top 5 Bad vendors by overspending:**

• Clark-Ward – R94,696,310

• Chavez, Reed and Cox – R54,935,268

• Gutierrez-Sanchez – R51,615,035

• Reeves PLC – R40,004,350

• Lee, Roberts and Lee – R37,941,482

<img src="Project%202%20-%20Municipality%20Risk%20Assessment/Images/Top_5_Bad_Vendors.PNG" width="400">

**Top 5 Good vendors by spending:**

• Clark-Cruz – R219,627,475

• Cunningham, Fisher and Smith – R196,259,475

• Holt and Sons – R184,145,730

• Wood, Beck and Wallace – R178,265,811

• Guzman-Miller – R168,108,850

<img src="Project%202%20-%20Municipality%20Risk%20Assessment/Images/Top_5_Good_Vendors.PNG" width="400">

## Insights Deep Dive

**Contract Classification:**

• 63% of contracts were flagged as Bad.

• Good contracts had zero irregular spend and consistently met approved budgets.

**Financial Exposure:**

• Overspending totaled R1.19 bn, concentrated among a small group of vendors.

• Departments with frequent deviations and missing MBD documents contributed disproportionately to financial risk.

**Vendor Risk:**

• Top overspending vendors represent the largest share of Bad contracts.

• High-performing vendors delivered large budgets without operational or financial flags.

## Takeaways & Recommendations

**Systemic Oversight Gaps**

Takeaway: R1.19 bn overspent (9% above budget) across flagged contracts indicates weak financial controls.
Recommendation: Implement tighter budget enforcement, automated spend tracking, and escalation protocols when variance exceeds 5%.

<img src="Project%202%20-%20Municipality%20Risk%20Assessment/Images/Total_Spend_By_Dept.PNG" width="600">

**Vendor Risk Concentration**

Takeaway: A small group of vendors account for most overspending (Clark-Ward alone: R94m).
Recommendation: Conduct enhanced due diligence and audits on repeat overspend vendors; consider blacklist/review procedures.

**Contract Management Failures**

Takeaway: 63% of contracts had operational red flags (missing documents, delays, premature completion).
Recommendation: Enforce MBD documentation at award, implement milestone reporting, and verify completion independently.

**High-Performing Vendors Exist**

Takeaway: Vendors like Clark-Cruz, Cunningham, and Holt managed large budgets successfully.
Recommendation: Establish a “preferred vendor” program and benchmark practices for underperforming vendors.

**Strategic Impact**

Takeaway: Bad contracts erode trust, drain budgets, and reduce service delivery.
Recommendation: Maintain a real-time audit dashboard to monitor risk, overspending, and vendor exposure proactively.

## Assumptions & Limitations

• Dataset represents a snapshot of 500 municipal contracts; external contracts not included.

• Irregular spend was only recorded for Bad contracts.

• Risk scores are calculated based on available contract metadata; external fraud indicators are not included.

• Visualizations assume accurate data entry and do not model external market factors.
