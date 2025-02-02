# A/B test analysis: website variations

## **Dataset overview**
This dataset contains data on **sales** and **customer satisfaction** before and after an intervention, as well as purchase data for control and treatment groups. 
Source: [Kaggle](https://www.kaggle.com/datasets/matinmahmoudi/sales-and-satisfaction).

## **Objective**
The goal of this analysis is to assess the effectiveness of the **website intervention** by comparing **Sales** and **Customer Satisfaction** metrics between the control and treatment groups. The main objective is to:
- Test if the intervention had a statistically significant effect on sales and customer satisfaction.
- Compare the performance of different customer segments (Low, Medium, High) across both groups.
  
## **Recommendations**
- **Apply treatment to all Segments**: since the treatment had a positive impact on sales, it should be extended to all customer segments.
- **Focus on High-Value customers**: the **High Value** segment showed the most significant improvement in sales, and further targeted optimization could increase this benefit.
- **Monitor customer satisfaction**: since the experiment did not show a significant improvement in customer satisfaction, ensure that any future changes do not negatively impact the customer experience.
  
## **Key findings**
- **Sales**: significant differences in sales were observed between the **control** and **treatment groups**, particularly in the **High Value** customer segment.
- **Customer satisfaction**: no significant difference in overall customer satisfaction was found, although variations existed between customer segments.

### **Features:**
- **Group**: Indicates whether the data point belongs to the Control or Treatment group.
  - Categories: Control, Treatment
- **Customer_Segment**: Categorizes customers based on their value.
  - Categories: High Value, Medium Value, Low Value
- **Sales_Before**: Sales figures before the intervention.
  - Data Type: Numerical
- **Sales_After**: Sales figures after the intervention.
  - Data Type: Numerical
- **Customer_Satisfaction_Before**: Customer satisfaction scores before the intervention.
  - Data Type: Numerical
- **Customer_Satisfaction_After**: Customer satisfaction scores after the intervention.
  - Data Type: Numerical
- **Purchase_Made**: Indicates whether a purchase was made after the intervention.
  - Categories: Yes, No


## **Analysis steps**
- **Data preprocessing and EDA**: cleaned the dataset by handling missing values, and transformed the data for analysis.
- **Assumptions checks**: performed tests for normality, homogeneity of variance, and outliers before proceeding with statistical tests.
- **Statistical testing**: applied **Mann-Whitney U test** for non-normal data and **Two-Way ANOVA** to assess the effects of the intervention across different segments.
- **Post-Experimental analysis**: used **Tukey’s HSD** for multiple comparisons to identify specific group differences.

### **Conclusion**
This analysis provides actionable insights for enhancing the website's performance based on sales results. Future steps could involve deeper dives into specific customer segment behaviours, with a focus on maximising both customer satisfaction and sales.
