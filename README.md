# EscapeRoomFinal
Creating an escape room GUI themed game where player is stuck in a locked room with a view of four doors.
Game prompts you to use provided empty backpack.
Upon entering levels (doors) there will be items to collect in your backpack; hopefully the right item was chosen as you need
to complete the game with the correct items otherwise final level will notify GAME OVER.

Player chooses a door which has may or may not have an obstacle to solve prior to entering.

First door's puzzle is a keycode in which needs to be guessed corectly for entry.
The items listed outside of the door are in alphabetical order cluing to the keycode password. (it's 1234).
A text field will be displayed to enter answer.
Upon entering, a text file is read with a clue as to which item to pick.
If successful and upon entry *choose item*
The items are busts of Shakespeare and Beethoven. Hopefully player has chosen Shakespere. 

The next door is not locked. Free entry.
Within door #2, upon entry *choose item*
A clue is displayed; pick the red or blue key.
A text field will be displayed to enter answer.
Hopefully player has chosen the red key.

Door three is unlocked as well but player is still trapped.
Within door #3, upon entry *choose item*
A clue is displayed; pick the crowbar or lock pick.
A text field will be displayed to enter answer.
Hopefully player has chosen the lock pick.

Door four is the final door. 
Upon entering a view of your essential backpack is shown.
Text appears deciphering whether you have chosen wisely to determine fate.

If clues were solved and correct items were chosen, YOU WIN.
If wrong items were chosen, GAME OVER.

Game is designed to play as many times as user chooses for win/lose outcome.

Met final requirements:
1. Project is a GUI using PyGame.
2. More than three functions used for project.
3. List is provided near top of code: list of rooms to go through and remove after "entering".
roomList = ("room1", "room2", "room3")
4. backpack is my dictionary. 
backpack = {
	      "key":"none",   #Red key or Blue key
        "tool":"none", #Lock Pick or Crowbar
	      "bust":"none"   #Shakespeare/Beethoven
	}
5. Modules used: tkinter, breezypythongui, pygame, & time. tkinter develops the GUI, 
breezypython creates game frame etc., pygame aids with images, and time helps with time.sleep 15(seconds) when timing out for game over.
6. "read" file used for door #1. "clue.txt"
7. Try and Except used to help with entering first room and buttons.
try:
       room1 = roomList.index(room1)
       doorOne()
 except ValueError:
       self.doorOneButton["state"] = "disabled"
8. Lots of if/else/elif/loops and data entry validation used throughout.
9. We did not use "dedent" in class, which is de indent to help with text display. Timing 15 seconds for game over with time.sleep(15) was used as well. Example: print(f"You've collected a {bust} bust, {key} key, and a {tool}.") to extract collected items and displayed for player was used.
10. GitHub was used. 
EscapeRoomFinal/projectFinal at main · Cglan012Ee/EscapeRoomFinal (github.com)

Reflection: I'm proud of accomplishing a concise game. I love my game idea and it was pleasing to create my idea with python. It was interesting trying to figure out which route to take to display images; the most difficult requirement to add was maybe try/except and debugging. I wish everything was perfect but it isn't quite there; this is my ultimate pitfall. I could add more obstacles to get into levels (doors).
