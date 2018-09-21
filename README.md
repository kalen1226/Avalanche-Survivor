Greetings. This is the official guide for the project Avalanche Survivor, a 2D Game that utilizes the SDL
library in C. Given that this project relies on grpahics, CS50 IDE cannot accomodate the use of this code to
execute the game. Therefore, before you can access this project, you must first download the Ubuntu virtual machine, whose instructions
can be found at https://builtvisible.com/the-ubuntu-installation-guide/

Upon having downloaded and set up the Ubuntu Virtual Machine, you must then create an account to be able to access the home screen of ubuntu.
Once you have done so, click on the purple icon with the circle inside in the left taskbar. That is the application
that will allow you to search your computer for the terminal needed to compile and run code on the virtual machine. Simply
search "Terminal," and click on the icon that has a black screen and is labeled "Terminal." That will open the terminal for you
so that you can officially compile and run code as you see fit. In addition, search for "Text Editor," and select the icon with the label
"Text Editor." Text Editor is the application that compliments the Terminal; it is where code can be written, and where you will have
access to the code of this project.

Having selected both "Terminal" and "Text Editor," open up the terminal. This is essentially your virtual machine. You will notice that you are currently not in any folders, as you have not yet downloaded
or created any folders to access. This project will be contained within a folder called sdl~seminar~master, a folder containing code that inspired my project. To download this folder
enter in the terminal git clone https://github.com/tlively/sd_seminar.git After that type in your terminal window "cd ~/sdl_seminar-master"
You will then be in the correct directory, which means you will be able to compile and run code pertaining to my project and this folder at will.
To access the Text Editor, type "gedit" into the terminal, and it will open
a blank page. That is because gedit simply open the text editor. To open up specific files, you would type "gedit ___," where the blank
is the name of the file containing the code you wish to look at.

Upon reaching the black text editor page, you can then copy the code for my project into the blank page. However, since ubuntu is its own software, you cannot simply copy and paste
all of my code into the text editor, so you will have to write the code word for word into the text editor. Unfortunately, I could not figure out how to copy words from Windows and paste it into
the Ubuntu's terminal or text editor, as whenever I use the keyboard commands or even right-clicking, I am unable to paste anything into the Ubuntu virtual machine. I apologize
for this inconvenience in advance, as my source code is well over 200 lines long. However, there is an alternative way to copy and paste the code into the text editor. Copy and and paste my source code
into an email and send it to yourself on your Windows or Mac laptop. Because Ubuntu is its own  virtual machine, you can access the Internet within Ubuntu as well.
Looking at the taskbar to the right again in Ubuntu, click on the Firefox icon two icons below the purple icon. This will allow you to acess Firefox. From there, you can
use Firefox's search engine to lookup your email website, and then pull up the email you sent to yourself when you were either in Internet Explorer, Google Chrome, Safari etc.
You can then copy the source code from there and then paste it inside the text box.

Once you have transferred all of my source code from CS50 IDE to the text machine, be sure to click the "Save" button at the top right of the screen, which will take you
to a window that allows you to type in the name of the program you wish to save. Save the game as "mygame.c," and save it under the folder
"sdl_seminar-master." That way, when you refer to the program from the terminal window, the program will be in the directory you
are currently in. Now that you have saved the source code for Avalanche Survivor, you are now able to compile the code. However, before you run the code, you must save the two images to be used
as sprites in the game. The links to each sprite are provided in the sources I have listed in resources.md. Within Ubuntu, search these links to find the images, and once
you have found them, save them both as .png files in the folder sdl_seminar-master, and within that folder, save them under resources. This will allow you to insert those saved images into the proper lines
of the source code so that they will appear. The names of these images you have saved is up to you. On line 69 of mygame.c, there is an IMG_load function
to the right, with the file of my image passed into it in parentheses. Delete "resources/5203-Galaga_Alien_Ship_C.png" and type in the name of
your file for the Galaga Ship Sprite in the following format:
         "resources/(filename).png"
Follow this same step for line 111 of mygame.c, except that you will pass in the file of the player sprite: "resources/(filename).png"


Now, to be able to compile in the terminal, you must close the text editor window to be able to type commands into the termianl. Once you have close the text editor window,
you can compile mygame.c by typing in the terminal "make SRCS=mygame.c" which will compile mygame.c for you. Upon compiling it, you will be greeted with two warnings
pertaining to the code. They do not affect the program whatsoever, as they are unique to SDL, so you can ignore them. Next, type in
"./game" to run the code.

As a result, a black window presenting the player sprite will open. You can use the arrow keys to move the sprite, or you can use
the A, S, D, and W keys to do so as well. In this game, you will be controlling a sprite that must avoid the incoming Galaga ships that are spawning
from the bottom of the screen. The game is designed to go on indefinitely, so there is no end to the enemies. If you collide with any of the Galaga ships
the game will freeze all animations on the screen. Do not be alarmed. This is just to let you know that the you have lost. To restart the game,
simply close the window, type ./game in your terminal, and a new black window with your character will appear, allowing you to replay the
game. This concludes the instructions on how to run the source code.




