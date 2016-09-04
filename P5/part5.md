## Part 5: Adding Alerts!

Our app is almost done. You can already play and enter guesses until you get the right number. However, you can't really see if you've won or if your guess is too high or too low. In this part of the tutorial, we will be adding some alerts, as well as updating our `guessLabel` to notify the player on the state of the game.

### guessLabel

First, we want to make sure that our `guessLabel` changes when the player's guess is higher or lower than the number to guess. If the player's guess is higher, we'll ask for a lower number, and vice versa. Update your `validateGuess` function to look like this:

```swift
func validateGuess(guess: Int) {
    if guess < lowerBound || guess > upperBound {
        print("Your guess should be between 1 and 100!")
    } else if guess < numberToGuess {
        guessLabel.text = "Higher! ⬆️"
    } else if guess > numberToGuess {
        guessLabel.text = "Lower! ⬇️"
    } else {
        print("You win!")
        numberOfGuesses = 0
        generateRandomNumber()
    }
}
```   
As you can see, `guessLabel` will now show "Higher! ⬆️" or "Lower! ⬇️", depending on the player's input. When you run your app and play, you will see something like this:

<p align="center"> <img src="/images/higher.png" align="center"> </p>

<p align="center"> <img src="/images/lower.png" align="center"> </p>

### UIAlertController

### Next Time
