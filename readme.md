# iChoose-Beta 0.1.2
## GitHub Author: cp-daniel-mccoy

iChoose is a simple program that randomly selects from a list of options for you.

This program is written in rust and is used to demonstrate basic rust functionality including user input, basic crate usage, loops, vectors, and other basics.

To use this program:
> **cargo run**

How this program works:

* 1.) It will ask you to enter some options (ex. places to eat). Enter each option line by line.
* 2.) Each time you enter a line, it will check to see if it's empty or if you typed "done".
* 3.) It will add each line of valid input into a vector until "done" is entered.
* 4.) It then generates a random number between 0 and the length of your options list.
* 5.) Forces the data types between i32 and usize to use the generated number to reference the vector.
* 6.) Displays a random selection from your list.

Planned Updates:

* 1.) Better error handling.
* 2.) Wrap in a loop to ask if you want to run again or exit.
* 3.) Some kind of frontend.
* 4.) A list loading/saving system to select from pre-existing lists.

Known Issues:

* 1.) If you only enter 2 options only the first gets selected. This will be addressed by changing the source of the random number to an independently generated one instead of using the thread based generator.
* 2.) The program currently crashes if you type "done" before entering input for the list or if you enter blank input. This is being handled currently by minor input validation to display the error but it needs further action. This will be addressed by better input validation and wrapping the program in a loop.
* 3.) If you only enter 1 option and type "done" the program currently crashes with an unhandled thread panick. This will be addressed by adding input validation and wrapping the program in a loop.

Disclaimer:

At the time of creation this program was one of my first written in Rust. Therefore, this program is subject to errors, inefficiencies, and experimental changes throughout development.

I hope you enjoy using or modifying this, or that you learned or valued from it in some way or another.

GitHub Author: cp-daniel-mccoy
