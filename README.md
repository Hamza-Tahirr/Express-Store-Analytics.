# Express Store Analytics

## Overview

**Express Store Analytics** analyzes an experiment conducted by **Company ABC** aimed at improving online grocery shopping through **automation** and **AI**. The experiment introduced the **'Express Store'** feature, offering a subset of products with faster delivery compared to the traditional shopping experience. The primary goal was to determine the impact of these variants on customer behavior, total spend, and unit economics.

## Experiment Design

The experiment involved three groups:

- **Variant 0 (Control Group)**: Standard online shopping with no 'Express Store' option.
- **Variant 1**: Offered an 'Express Store' with faster delivery but a narrower selection of products.
- **Variant 2**: Offered an 'Express Store' with faster delivery and a lower minimum basket size ($10 vs. the usual $35).

## Key Concepts & Column Definitions

- **experiment_group / grp_code**: The experiment group assigned to each customer.
- **assignment_date**: The date a customer was assigned to a group.
- **address_type**: Indicates whether the customer’s address is a business or residential one.
- **express**: Whether the customer is a member of Company ABC’s express program.
- **loyalty**: Whether the customer is part of the retail partner's loyalty program.
- **order_placed**: The total number of orders placed since assignment.
- **avg_order_value**: The average value of orders placed.
- **total_spend**: The total amount spent by the customer since assignment.

## Key Questions Addressed

1. **What insights can be drawn from the experiment?**
   - **Variant 0** serves as the baseline for customer behavior without an 'Express Store'.
   - **Variant 1** helps to understand how customers respond to faster delivery but limited product variety.
   - **Variant 2** examines the impact of a reduced minimum basket size on customer behavior and spending.

   **Recommendation**: Focus on strategies to increase **total spend** and perform a detailed **cost-benefit analysis** for smaller basket sizes, particularly in Variant 2.

2. **How reliable are the findings?**
   - Perform statistical tests (e.g., t-tests, ANOVA) to assess **statistical significance**.
   - Ensure sample sizes are large enough for meaningful insights.
   - Account for potential confounding factors such as express membership, loyalty programs, and address type.

3. **How should unit economics be assessed?**
   - Analyze the impact of delivery costs on smaller orders (Variant 2).
   - Evaluate the feasibility of rolling out variants based on profit margins at various customer spending thresholds (e.g., 5%, 10%, 20%).

4. **Next Steps**:
   - **Further Analysis**: Segment data by customer loyalty, express membership, and order frequency.
   - **Additional Data**: Collect more detailed information on delivery costs and customer satisfaction.
   - **Operational Scalability**: Ensure that the express store model can scale effectively without operational inefficiencies.

## Data Visualizations

Key visualizations used in the analysis include:

1. **Bar Plot**: Total spend by variant.
2. **Bar Plot**: Average number of orders placed per variant.
3. **Bar Plot**: Average order value by variant.
4. **Count Plot**: Sample size by experiment group.
5. **Bar Plot**: Profit by variant at different revenue cutoffs (5%, 10%, 20%).
6. **Box Plot**: Total spend by variant and loyalty program participation.
7. **Box Plot**: Total spend by variant and express membership participation.
8. **Box Plot**: Orders placed per variant and address type.
9. **Scatter Plot**: Order frequency vs. average order value by variant.
10. **Histogram**: Distribution of order sizes in Variant 2.
11. **Bar Plot**: Profit by variant considering additional delivery costs.
12. **Summary Plot**: Total spend, average order value, and order frequency by variant.
13. **Line Plot**: Profitability by variant across revenue cutoffs.
14. **Scatter Plot**: Operational impact (order size vs. total cost).

## Technologies & Libraries

This project utilizes the following libraries for analysis and visualization:

- **Prophet**: Time series forecasting.
- **PyCaret**: Machine learning and automated model building.
- **Seaborn**: Statistical data visualization.
- **Matplotlib**: General-purpose plotting.
- **Statsmodels**: Statistical models.
- **Pandas**: Data manipulation and analysis.
- **Numpy**: Numerical computations.

### Installation

To install the necessary dependencies, run the following command:

```bash
pip install -r requirements.txt
```

## Key Findings

1. Variant 2: Increased order frequency due to the reduced basket size, but profitability is a concern due to higher delivery costs for small orders.
2. Variant 1: Faster delivery led to increased customer spend, though operational costs for fast delivery need careful evaluation.
3. Statistical tests confirmed that the differences between variants are significant, with a large enough sample size for valid conclusions.

## Conclusion

The Express Store Analytics project offers actionable insights into how different versions of the 'Express Store' impact customer behavior, spending, and profitability. To ensure sustainable growth, future rollout strategies should balance faster deliveries, minimum basket size, and unit economics.

## Repository

The full project and analysis can be found in the repository below:

- Jupyter Notebook

## How to Contribute

I welcome contributions to this project! If you'd like to get involved, you can:

1. Open an Issue: If you encounter a bug or have a feature request, feel free to open an issue in the repository.
2. Submit a Pull Request: If you'd like to contribute code, fork the repository, make your changes, and submit a pull request.
   **All contributions are welcome!**


### Key Sections Included:
1. **Overview**: Introduces the purpose and scope of the project.
2. **Experiment Design**: Details the three experimental groups involved.
3. **Key Concepts & Column Definitions**: Explains the dataset terminology.
4. **Key Questions Addressed**: Discusses the core questions the analysis aimed to answer.
5. **Data Visualizations**: Lists the key visualizations used to analyze the data.
6. **Technologies & Libraries**: Outlines the key tools used for the project.
7. **Installation Instructions**: Provides instructions for installing dependencies.
8. **Key Findings**: Summarizes the main takeaways from the analysis.
9. **Conclusion**: Wraps up with overall conclusions about the experiment's success and considerations for future steps.
10. **Repository Link**: Directs readers to the full project repository.
11. **How to Contribute**: Provides guidance on how others can contribute to the project.

This version is complete and includes all sections requested. Let me know if you need further adjustments!
