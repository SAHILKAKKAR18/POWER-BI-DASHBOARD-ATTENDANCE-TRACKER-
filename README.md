# POWER-BI-DASHBOARD-ATTENDANCE-TRACKER-
📌 Power BI Project: Employee Attendance Tracker
Successfully built a dynamic Attendance Tracker Dashboard using Power BI, integrating cleaned Excel datasets and calculated KPIs for monthly performance insights.
🔧 Key Highlights:
Cleaned and transformed raw Excel data using Power Query and key Excel functions (e.g., IF, VLOOKUP, TEXT, NETWORKDAYS)
Visualized attendance metrics: Present, Absent, Leave, Weekoffs, Paid Days
Automated salary calculations with deduction logic based on attendance
Delivered interactive dashboards for HR and payroll teams with slicers by employee and month
📈 Tools Used: Power BI, Excel, DAX, Power Query
 ✅ Outcome: Streamlined attendance reporting and salary forecasting for 20+ employees across 12 months

📊 Key Performance Indicators (KPIs)
These are the most critical metrics tracked across employees and months:
1. Attendance Metrics
Present Days: Indicates employee reliability and work commitment.
Absent Days: Useful for identifying attendance issues or patterns.
Leave Days: Helps track planned time off and leave policy usage.
Weekoff Days: Standard non-working days, useful for payroll calculations.
2. Payroll Metrics
Paid Days: Total days considered for salary payout (Present + Leave).
Salary: Monthly gross salary assigned to each employee.
Per Day Salary: Derived from monthly salary ÷ Paid Days.
Deduction: Salary lost due to absences or unpaid leave.
Total Salary: Final payout after deductions.

END OF MONTH  - =EOMONTH(START DATE,0)
MONTH WISE DATE  - =IF((DATE<MONTH OF LAST DATE(F4),DATE+1,""))
WEEK OFF  -  =(COUNTIF(ALL DATE(F4),"SUNDAY"))
TOTAL PARSENT  =COUNTIF(ALL DATE,"P")
TOTAL ABSENT  =COUNTIF(ALL DATE,"A")
TOTAL LEAVE  =COUNTIF(ALL DATE,"L")
TOTAL DAYS   =DATEDIF((START DATE,LAST DATE,"D")+1)
PAID DAYS    =(TOTAL DAYS-ABSENT)
PER DAYS SALARY  = (SALARY/PAID DAYS)
DEDUCTION       =(PERDAY SALARY*ABSENT)
TOTAL SALARY    =(PER DAY SALARY*PAID DAYS-DEDUCTION)

🔍 Key Insights & Observations
✅ High Performers
Employees like Aditya Shekhawat, Priya Desai, and Riya Kaur consistently show high attendance and receive full salaries across months.
Meera Nair and Siddharth Bansal also maintain near-perfect attendance.
⚠️ Attendance Concerns
Karan Malhotra and Isha Chauhan show frequent absences or leaves, leading to notable salary deductions.
Rohan Verma and Nisha Gupta have fluctuating attendance, impacting their net salary.
💰 Salary Distribution
Salaries range from ₹15,000 to ₹85,000 monthly.
Highest earners: Nisha Gupta (₹85,000), Karan Malhotra (₹65,000), Aditya Shekhawat (₹65,000).
Lowest earners: Aanya Khanna (₹15,000), Tanvi Goyal (₹15,000).
📉 Deduction Trends
Deductions are directly tied to unpaid absences.
Months with more holidays (e.g., February, June) show fewer deductions due to fewer working days.
🔚 Conclusion
This project showcases how combining Excel-based data cleaning with Power BI visualization can transform raw attendance logs into actionable insights. From tracking employee presence to automating salary deductions, the dashboard delivers clarity and efficiency for HR and payroll teams. It’s a great example of how data storytelling can simplify decision-making and elevate operational transparency.
