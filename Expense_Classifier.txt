# Assignment 1 expense classifier

income = float(input("Enter your monthly income: "))
expenses = float(input("Enter your monthly expenses: "))


remaining = income - expenses
expense_rate = (expenses / income) * 100

high_expense = expense_rate > 70

print("\nMonthly Income:", income)
print("Monthly Expenses:", expenses)
print("Remaining Money:", remaining)
print("Expense Rate:", expense_rate, "%") 	
print("High Expense:", high_expense)

if expense_rate <= 50:
    print("Expense Level: Low")
elif expense_rate <= 70:
    print("Expense Level: Moderate")
else:
    print("Expense Level: High, you need to lower your expense")
