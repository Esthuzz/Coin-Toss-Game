import random

def coin_toss():
    print("Welcome to the Coin Toss Game!")
    guess = input("Guess the outcome (Heads or Tails): ").lower()
    
    if guess != 'heads' and guess != 'tails':
        print("Invalid input. Please enter 'Heads' or 'Tails'.")
    
    result = random.choice(['heads', 'tails'])
    print(f"The coin landed on {result.capitalize()}!")
    
    if result == guess:
        print("Congratulations! You guessed it right!")
    else:
        print("Sorry, better luck next time!")

if __name__ == "__main__":
    coin_toss()
