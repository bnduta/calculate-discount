# calculate-discount
def calculate_discount(price, discount_percent):
    if discount_percent >= 20:
        return price * (1 - discount_percent / 100)
    return price

try:
    price = input("please enter original price of the item: ")
    discount_percent = float(input("enter the discount percentage: "))

    final_price = calculate_discount(price, discount_percent)
    print(f"The final price after discount (if applied) is: ${final_price:.2f}")
except ValueError:
    print("Invalid input. PLease enter numeric values for price and discount.")


    
    
