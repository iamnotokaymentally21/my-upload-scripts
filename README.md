i would like you to like this maybe a free request sometimes uh yeah my stuff is bad sometimes anyways heres a game thing 

import time

def introduction():
    print("Welcome to the Adventure Game!")
    time.sleep(1)
    print("You find yourself in a mysterious land. Your choices will determine your fate.")
    time.sleep(1)

def make_choice(options):
    print("Choose your action:")
    for i, option in enumerate(options, start=1):
        print(f"{i}. {option}")

    while True:
        try:
            choice = int(input("Enter the number of your choice: "))
            if 1 <= choice <= len(options):
                return choice
            else:
                print("Invalid choice. Please try again.")
        except ValueError:
            print("Invalid input. Please enter a number.")

def main():
    introduction()

    while True:
        options = [
            "Explore the forest",
            "Enter the cave",
            "Go back to the village",
            "Quit"
        ]
        choice = make_choice(options)

        if choice == 1:
            print("Import your text for exploring the forest here.")
            # Add code for the outcome of choice 1

        elif choice == 2:
            print("Import your text for entering the cave here.")
            # Add code for the outcome of choice 2

        elif choice == 3:
            print("Import your text for going back to the village here.")
            # Add code for the outcome of choice 3

        elif choice == 4:
            print("Thanks for playing! Goodbye.")
            break

if __name__ == "__main__":
    main()
