# calculator-project
v2
# Project Title

Bu proje, GitHub üzerinde commit yapmayı öğrenmek ve deneme yapmak için oluşturulmuştur.

## Proje Hakkında

Bu dosya, bir Python programıyla basit bir hesap makinesi örneği içermektedir. Kullanıcıdan iki sayı alır ve toplama, çıkarma, çarpma, bölme işlemlerini gerçekleştirir.

## Example Python Script

```python
def calculator():
    print("Welcome to the Calculator!")
    print("Choose an operation:")
    print("1. Addition")
    print("2. Subtraction")
    print("3. Multiplication")
    print("4. Division")

    try:
        operation = int(input("Enter the number of the operation (1-4): "))
        if operation not in [1, 2, 3, 4]:
            raise ValueError("Invalid operation.")

        num1 = float(input("Enter the first number: "))
        num2 = float(input("Enter the second number: "))

        if operation == 1:
            result = num1 + num2
            print(f"The result of addition: {result}")
        elif operation == 2:
            result = num1 - num2
            print(f"The result of subtraction: {result}")
        elif operation == 3:
            result = num1 * num2
            print(f"The result of multiplication: {result}")
        elif operation == 4:
            if num2 == 0:
                print("Error: Division by zero is not allowed.")
            else:
                result = num1 / num2
                print(f"The result of division: {result}")

    except ValueError as e:
        print(f"Invalid input: {e}")

# Run the calculator
calculator()

