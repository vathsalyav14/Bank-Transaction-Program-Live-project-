# Bank-Transaction-Program-Live-project-
# A simple Python ATM transaction simulation. The program welcomes the user, asks them to insert their card, enter the withdrawal amount, and provide a PIN. The transaction details are then saved to a file. Built to practice basic Python concepts like user input and file handling.

print("===== Welcome to ATM =====")

name = input("Enter your name: ")
print(f"Hello {name}, Welcome to our ATM")
input("Please insert your ATM card and press Enter...")

amount = input("Enter amount to withdraw: ")

pin = input("Enter your PIN: ")

file = open("transactions.txt", "a")
file.write("Name: " + name + ", Amount: " + amount + ", PIN: " + pin + "\n")
file.close()

print("Processing transaction...")
print("Please collect your cash: " + amount)
print("Thank you for using the ATM")
