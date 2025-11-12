# Dual-Audience-Decision-Tree-Analysis
This project explores how dealership sales and vehicle information can be used to predict whether a car purchase is dealer-financed or not. The goal was to understand what factors most influence financing decisions and how dealership teams might use this insight to improve financial outcomes and customer targeting.

The analysis uses a dataset containing real dealership transaction information, including vehicle details, lender types, down payments, and sale characteristics.
By applying a Decision Tree analysis, we aimed to identify key decision factors—such as vehicle make, year, and lender type—that influence whether a customer uses dealer financing.

What factors best predict whether a vehicle will be dealer-financed or paid through another method?

- Understanding these patterns helps dealerships:

- Focus marketing on customers most likely to use dealer financing

- Adjust inventory and lending partnerships based on buyer behavior

- Identify opportunities to improve conversion rates and reduce finance declines



**Before analysis, several data cleaning steps were performed:**

Removed identifiers (VIN Number, Salesperson, Manager names) to avoid data leakage.

Encoded categorical values (Make, Model, Dealership) into numerical form so they could be analyzed computationally.

Converted the target variable (“Finance Type”) into a binary form:

Dealer Financed = 1

Other Financing or Cash = 0

Split the dataset into training (75%) and testing (25%) groups, ensuring the same balance of finance types in both sets.

Three Decision Tree analyses were performed using different maximum depths: Shallow Tree Max Depth 3 / Medium Tree Max Depth 5 / Deep Tree Max Depth 10

The analysis compared training vs. testing accuracy to identify signs of overfitting and determine the ideal tree depth.

The analysis found that vehicle make, year, and lender are the biggest clues to how a deal will be financed. This can guide sales teams to focus effort where dealer financing is most probable.



**Recommendations**

Prioritize Makes and Models with higher dealer-financing likelihood when promoting finance specials.

Strengthen partnerships with lenders most associated with dealer-financed deals.

Use a simplified decision flow (based on the shallow tree) for finance managers. 



**Limitations**

The dataset does not represent all dealership transactions, and is only a snapshot in time - August 2025 and October 2025 and some categories were underrepresented, which limits model generalization.

Decision trees can overfit easily when too many features or levels are used.

The analysis shows correlation, not causation—so further validation would be needed before using results for financial decision-making
