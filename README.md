# calculator
def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    if y != 0:
        return x / y
    else:
        return "Error! Division by zero."

def  calculator():
    print("Select a arithmatic operation:")
    print("1. Add")
    print("2. Subtract")
    print("3. Multiply")
    print("4. Divide")

    choice = input("select one (1/2/3/4) : ")

    if choice in ['1', '2', '3', '4']:
        num11 = float(input(" enter 1st value: "))
        num2 = float(input("Enter 2nd value: "))

        if choice == '1':
            print(f"\n  {num1}\n+ {num2}\n= {add(num1, num2)}")
        elif choice == '2':
            print(f"\n  {num1}\n -{num2}\n= {subtract(num1, num2)}")
        elif choice == '3':
            print(f"\n  {num1}\n *{num2}\n= {multiply(num1, num2)}")
        elif choice == '4':
            print(f" {num1}/{num2}= {divide(num1, num2)}")
    else:
        print("this is simple caculator,plz enter valid no.")

if __name__ == "__main__":
    calculator()
