# Calc
# Financial Calculator in Python

# Input data
present_value = float(input("Enter the present value of the investment: "))
annual_rate = float(input("Enter the annual interest rate (as a %): "))
years = int(input("Enter the number of years: "))

# Convert annual rate percentage to a decimal
rate = annual_rate / 100

# Calculate future value
future_value = present_value * ((1 + rate) ** years)

# Output the result
print(f"The future value of the investment is: ${future_value:.2f}")
