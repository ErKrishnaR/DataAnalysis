# DataAnalysis
Finance Dashboard
Measures
1.	Title = "My Finance Dashboard"
2.	Total Income = CALCULATE(SUM(FinData[Value]),FinData[Type]="Income")
3.	Total Expense = CALCULATE(SUM(FinData[Value]),FinData[Type]="Expense")
4.	Total Saving = CALCULATE(SUM(FinData[Value]),FinData[Type]="Savings")
5.	Income LM = CALCULATE([Total Income],DATEADD(FinData[Date],-1,MONTH))
6.	Income Change MoM % = DIVIDE([Total Income],[Income LM])  
7.	Saving Targets = 0.25
8.	Expense % = DIVIDE([Total Expense],[Total Income])
9.	Saving % = DIVIDE([Total Saving],[Total Income])
