# def main():
    numbers = []
    while True:
        entry = input("Enter a number or press enter to quit: ")
        if entry == "":
            break
        try:
            numbers.append(float(entry))
        except ValueError:
            print("Please enter a valid number.")
    total = sum(numbers)
    average = total / len(numbers) if numbers else 0
    print(f"\nThe sum is {total}")
    print(f"The average is {average}")

if __name__ == "__main__":
    main()
