# The-Tech-Academy-Basic-C-Sharp-Projects.-
# Print the initial welcome message for the user
print("Welcome to Package Express. Please follow the instructions below.")

# Prompt the user for the package weight
weight = float(input("Please enter the package weight: "))

# Check if the package weight exceeds 50
if weight > 50:
    # Display an error message if the package is too heavy and exit the program
    print("Package too heavy to be shipped via Package Express. Have a good day.")
else:
    # Prompt the user for the package width
    width = float(input("Please enter the package width: "))

    # Prompt the user for the package height
    height = float(input("Please enter the package height: "))

    # Prompt the user for the package length
    length = float(input("Please enter the package length: "))

    # Calculate the sum of the package dimensions
    dimensions_total = width + height + length

    # Check if the dimensions total exceeds 50
    if dimensions_total > 50:
        # Display an error message if the package is too big and exit the program
        print("Package too big to be shipped via Package Express.")
    else:
        # Calculate the quote by multiplying dimensions and weight, then dividing by 100
        quote = (width * height * length * weight) / 100

        # Display the quote as a dollar amount formatted to two decimal places
        print(f"Your estimated total for shipping this package is: ${quote:.2f}")
        # Display a thank you message
        print("Thank you!")
