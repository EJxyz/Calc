# Calc
# Financial Calculator in Python

 # Financial Calculator in Python

def calculate_future_value(present_value, annual_rate, years):
    """
    Calculate the future value of an investment.
    
    Parameters:
    present_value (float): The initial amount of money invested.
    annual_rate (float): The annual interest rate as a percentage.
    years (int): The number of years the money is invested.
    
    Returns:
    float: The future value of the investment.
    """
    # Convert annual rate percentage to a decimal
    rate = annual_rate / 100
    # Calculate future value
    future_value = present_value * ((1 + rate) ** years)
    return future_value

# Example usage:
if __name__ == "__main__":
    # Input data
    present_value = float(input("Enter the present value of the investment: "))
    annual_rate = float(input("Enter the annual interest rate (as a %): "))
    years = int(input("Enter the number of years: "))
    
    # Calculate future value
    future_value = calculate_future_value(present_value, annual_rate, years)
    
    # Output the result
    print(f"The future value of the investment is: ${future_value:.2f}")
