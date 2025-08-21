Here’s a step-by-step solution to the problem, perfect for beginners learning how to write and use functions in Python. 👇

✅ Define the function calculate_discount

We create a function that accepts:

price: the original price of the item.

discount_percent: how much discount to apply.

Inside the function:

If the discount is 20% or more, apply it to the price.

If the discount is less than 20%, return the original price.

def calculate_discount(price, discount_percent):
    if discount_percent >= 20:
        discount_amount = (discount_percent / 100) * price
        final_price = price - discount_amount
        return final_price
    else:
        return price

# Get input from user
price = float(input("Enter the original price of the item: "))
discount_percent = float(input("Enter the discount percentage: "))

# Calculate final price
final_price = calculate_discount(price, discount_percent)

# Display the result
if final_price < price:
    print(f"🎉 Discount applied! Final price is: ${final_price:.2f}")
else:
    print(f"No discount applied. Final price is: ${final_price:.2f}")
 
