# HR Data Analysis

## Research Questions
- Which job title is leaving the most?

- What are the determinants of employee job satisfaction?
- What are the key factors influencing employee attrition?


I conducted an analysis to determine what factors influencing employee job satisfaction at IBM. Job Satisfaction is measured using a score of 1 to 5. The purpose of this analysis is to see if IBM can do anything to keep satisfaction rates high. I used a linear regression model to see each variable’s impact. 

image 1


The linear regression model shows some surprising results. Only 2 variables returned as significant. Employees with a higher hourly rate, actually had slightly lower levels of job satisfaction. This could be because higher paying positions may have more stressful jobs at IBM. The more companies an employee worked at previously also resulted in slightly lower job satisfaction scores. Overall, not much could be proven when determining the impact of these variables on job satisfaction. 

Next, I decided to look at employee attrition. The purpose of this analysis was to determine what factors are associated with employees leaving the company, and how IBM could try to improve employee retention. Because attrition is a binary variable, logistic regression was used. 




image 2


The results of this analysis are less surprising.  Let’s go through each variable.

Age
 - Interpretation: For every one-year increase in age, the log odds of attrition decrease by 0.03083, holding other variables constant.
 - Effect: As employees get older, they are less likely to leave the company. This makes sense as older employees may be more settled in their positions.

DistanceFromHome
- Interpretation: For each unit increase in the distance from home (likely measured in miles or kilometers), the log odds of attrition increase by 0.02728.
- Effect: Employees who live farther from their workplace are more likely to leave the company, perhaps due to commuting difficulties or dissatisfaction with work-life balance.

JobSatisfaction 
- Interpretation: For each unit increase in job satisfaction (likely on a scale), the log odds of attrition decrease by 0.2735.
- Effect: Higher job satisfaction significantly reduces the likelihood of an employee leaving. This is a strong predictor, as more satisfied employees are less likely to quit.

WorkLifeBalance 
- Interpretation: For each unit increase in work-life balance (likely on a scale), the log odds of attrition decrease by 0.2441.
- Effect: Employees with a better work-life balance are less likely to leave. This suggests that work-life balance is an important factor in retention.

YearsAtCompany 
- Interpretation: For each additional year an employee stays with the company, the log odds of attrition decrease by 0.04513.
- Effect: Employees who have been with the company longer are less likely to leave, potentially due to increased loyalty or benefits from tenure.

MonthlyIncome 
- Interpretation: For each unit increase in monthly income, the log odds of attrition decrease by 0.00007188.
- Effect: Higher income is associated with a lower likelihood of attrition, likely because better-paid employees may feel more valued or have fewer financial incentives to leave.

Age, Job Satisfaction, Work-Life Balance, and Years at Company are significant negative predictors, meaning increases in these factors reduce the likelihood of attrition. Distance from Home increases the likelihood of attrition, while Monthly Income reduces it. These insights can help the IBM focus on improving job satisfaction, work-life balance, and compensation to reduce attrition rates.
