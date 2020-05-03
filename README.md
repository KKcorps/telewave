# telewave

Forked from [gjeuken/telewave](https://github.com/gjeuken/telewave)

[Access it here](https://umanghome.github.io/telewave/)

# Instructions

* [Good video explaining the game](https://youtu.be/4lwGkSiEHeA)
* One person starts this on their computer and shares their screen.
* As soon as the host clicks on "Copy Peek URL", a link is copied to the clipboard, which can be shared with the psychic.
* The psychic visits the link and clicks on Peek.
* The psychic then gives the clue to the team.
* The host will place the marker at the requested position.
* The host clicks on "Guess".
* Points are then assigned by the host.

# Misc
* The basis of this implementation is that **each seed generates a unique board**.
	* This means that when two people input the same seed, they will have the same target position and words.
	* It is possible then for the **clue giver** to open the board on his own computer/phone and **peek** at the target without having to share it in the videocall.
* Functions:
	* Seed: generates a unique board. The seed can be **any combination of numbers and letters**. (Tip: using words makes it easier to share the seed.)
	* New clue: generates a new random seed.
	* Copy Peek URL: Copies to clipboard a URL that can be shared wit the psychic.
	* Guess: Compares your current position of the dial against the target, and shows you how many points you got.
	* Peek: reveals the target.
	* Clear: Erases the target and guess from the board.
	* Percentages: Toggles the display of the percentages under the dial. (The official rulebook advises against using percentages to discuss the dial, yet I've found that they make playing via videocall much easier.)
	* There are two manual score boards at the bottom for keeping track of your points.
