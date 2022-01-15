# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG
![Screen Shot 2022-01-15 at 12 59 05 PM](https://user-images.githubusercontent.com/16244455/149637515-f80a3426-8fae-4589-b18b-ab4390533849.png)
- Vehicle length and ground clearance have a significant impact on MPG for these cars
- Because the p-value of 5.35e-11 is much smaller than the 0.05 significance value, we can assume the slope of the line is not 0
- Because the Multiple r-value is 0.7149, this linear model does predict mpg effectively

## Summary Statistics on Suspension Coils
![Total Summary](https://user-images.githubusercontent.com/16244455/149638801-1362b63c-5189-41eb-9204-47f48eb46b18.png)
![Lot Summary](https://user-images.githubusercontent.com/16244455/149638803-47f3f2c9-8d1e-43b7-8e3e-cd0788206feb.png)

While the overall variance of 62 is well under the 100 variance limit, Lot 3 is at a 170 PSI variance, well above the limit.  Addressing the issues at this lot would likely bring down the overall variance limit significantly

## T-Tests on Suspension Coils
![Total T-Tests](https://user-images.githubusercontent.com/16244455/149638990-658d0f67-b1e5-45f0-b950-c866cc3a1896.png)
![Lot T-Tests](https://user-images.githubusercontent.com/16244455/149638995-e3766cf0-131b-494d-881d-8d3d8ca56088.png)

- Similar to the last analysis, the overall p-value of 0.06 is above the 0.05 signifiance value, the overall manufacturing lots are not statistically different from the population mean of 1500
- However, when looking at the individual lots, Lot 3 has a p-value of 0.04, under the signficance value, indicating that this lot is statistically different from the population mean

## Study Design: MechaCar vs Competition

In order to understand strengths and gaps in the market as it relates to ongoing costs, I would evaluate MechaCars cost, repair costs, mpg on city and highway against different car types (ie sedan, compact, etc) vs our competitors

### Metrics to test
- Cost
- Repair Cost
- City MPG
- Highway MPG

### Hypothesis

- H0 (Null Hypothesis): MechaCar's overall vehicle costs are no different from its competitors
- Ha (Alternative Hypothesis): MechaCar's overall vehicle costs are different from its competitors

### Statistical Test
Because we will have multiple samples a two-sample t test can be used.  Additionally, because there will be categorical data, a chi-squared test can also be used.

### Data Needed
The data we will need is:
- Vehicle class
- Initial Cost
- Repair Costs by Year
- MPG by Year
