# small_bank
taking some amount as a deposite amount and then widraw some of the money. 
balance = 0.0

print("welcome to My bank")
def checking_balance():
    print(f"Your remaining balance is:{balance}")




def deposit(amount):
    global balance
    if amount > 0 :
        balance += amount
        print(f"Your Deposited amount is: {amt}")
        print(f"Your total amount is {balance}")
    else :
        print("can't deposit negative amount")

 
def withdraw(amount):
    global balance
    if amount <= 0:
        print("Something Error! Please Try Again.")
    elif amount> balance:
        print('Insufficient Balance.')
    else:
        balance -= amount
        print(f"Your withdrawal money is: {amt1} ")
        print(f"Your total amount is {balance}")


while True:
    print("1. Check Your balance")
    print("2. Deposit an amount")
    print("3. Withdraw an amount")
    print("4. Quit")
    choice = input("Enter your choice (1-4):")

    if choice == "1":
        checking_balance()
    elif choice == "2":
        amt = float(input("Enter your amount:"))
        deposit(amt)
    elif choice == "3":
        amt1 = float(input("Enter your amount:"))
        withdraw(amt1)
    elif choice == "4":
        break
    else :
        print("Invalid choice!!! Re-try.")
    
print("Thank you for banking with us,come Again.")
