# python-fortune-teller-game-
print("\n\t\t\t\tThe Fortune Teller!")
print("You will select a color and a number, and I will tell you what your future holds for you!")

c = input("\nDo you want to play the game? ('y' or 'n'): ")

while c.lower() == 'y':
    color = input("\nChoose a color from - Yellow, Green, Blue, Red: ").strip().lower()
    
    while color not in ['yellow', 'green', 'blue', 'red']:
        print("Only colors Yellow, Green, Blue, or Red are allowed!")
        color = input("Please choose again: ").strip().lower()
    
    if color in ['yellow', 'green']:
        number = input("Select a number from - 1, 2, 5, 6: ")
        while number not in ['1', '2', '5', '6']:
            print("Only numbers 1, 2, 5, 6 are allowed!")
            number = input("Please select again: ")
        
        if number == '1':
            print("\nWorried about your future? Don't worry! You'll 100% get what you want! Be patient!")
        elif number == '2':
            print("\nYou will become a millionaire at the age of 35!")
        elif number == '5':
            print("\nYou will have a great family with 10 kids!")
        elif number == '6':
            print("\nYou will become famous, and everyone will love you!")
    
    elif color in ['blue', 'red']:
        number = input("Select a number from - 3, 4, 7, 8: ")
        while number not in ['3', '4', '7', '8']:
            print("Only numbers 3, 4, 7, 8 are allowed!")
            number = input("Please select again: ")

        if number == '3':
            print("\nYou will have a happy life for at least 100 years!")
        elif number == '4':
            print("\nYou will become a successful doctor one day!")
        elif number == '7':
            print("\nAll your dreams will come true, just be patient!")
        elif number == '8':
            print("\nYou're lucky! You'll have it all one day!")

    c = input("\nDo you want to play again? ('y' or 'n'): ")
