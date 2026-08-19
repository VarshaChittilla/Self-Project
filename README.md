# Self-Project
#Define the menu of a cafe
menu = {
    'Boba Tea': 120,
    'Matcha Latte':250,
    'Smores Frappucino':200,
    'Dalgona Coffee':170,
    'Brewed Coffee':100,
    'Dragon fruit Smoothie':300,
}

#Greet
print("Welcome to Kiki's Cafe")
print("Boba Tea: Rs.120\nMatcha Latte: Rs.250\nSmores Frappucino: Rs.200\nDalgona Coffee: Rs.170\nBrewed Coffee: Rs.100\nDragon fruit Smoothie: Rs.300")

order_total = 0
#120 + 200 = 320

item_1 = input("Enter the item you want to order:")
if item_1 in menu:
    order_total += menu[item_1] #0 + 120
    print(f"Your item {item_1} has been added to your order ")
    
else:
        print(f"Ordered item {item_1} is not available yet!")
        
another_order = input("Do you want another item? (Yes/No)")
if another_order == "Yes":
 item_2 = input("Enter the name of second item = ")
if item_2 in menu:
    order_total += menu[item_2]
    print(f"Item {item_2} has been added to order")
else:
    print(f"Ordered item {item_2} is not available!") 
print(f"The total amount of items to pay is {order_total}")
