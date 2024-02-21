import random

def hangman():
    words = ['python', 'programming', 'hangman', 'game', 'formative']
    word = random.choice(words)
    guessed_letters = []
    tries = 6
    
    while tries > 0:
        guessed_word = ""
        for letter in word:
            if letter in guessed_letters:
                guessed_word += letter
            else:
                guessed_word += "_"
        
        print("Guess the word: ", guessed_word)
        print("Tries remaining: ", tries)
        
        if guessed_word == word:
            print("Congratulations! You guessed the word correctly!")
            return
        
        guess = input("Enter a letter: ")
        
        if guess in guessed_letters:
            print("You already guessed that letter. Try again.")
        elif guess in word:
            print("Good guess!")
            guessed_letters.append(guess)
        else:
            print("Wrong guess!")
            tries -= 1
            guessed_letters.append(guess)
        
        print()
    
    print("You ran out of tries. The word was", word)

hangman()
