print("Welcome to the calculator")

# Get the total bill, number of people, and tip percentage
total_bill = float(input("Enter the total bill for the lunch: "))
no_of_people = int(input("How many people will split the bill: "))
per = int(input("What percentage tip would you like to give (5, 10, 15, 20, 25, 30, 35, 40): "))

# Calculate the tip amount
tip_amount = (per / 100) * total_bill

# Calculate the total bill including the tip
total_bill_with_tip = total_bill + tip_amount

# Calculate how much each person should pay
total_bill_per_person = total_bill_with_tip / no_of_people

# Display the result
print(f"Each person should pay: ${total_bill_per_person:.2f}")
