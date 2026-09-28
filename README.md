Kernel Panic (haunted_terminal)

A short, browser-based horror game that plays out inside a fake Linux terminal. Explore files, read a stranger's notes, and try not to look at the screen too closely.

Built with plain HTML, CSS and JavaScript. It is one file with no dependencies and no build step.

Content warning: contains sudden loud audio, flashing/flickering visuals, screen shake and jump scares. Not suitable for anyone sensitive to these. Play with headphones at a moderate volume.

![img of the game](image.png)


Download kernel.panic and run on any browser

How to Play

Type commands into the prompt and press Enter.

Command	What it does
help	Lists available commands
whoami	Shows who you are logged in as
ls	Lists files in the current folder
cat FILE	Prints a file, e.g. cat notes.txt
clear	Clears the screen
restart	Reloads the session from scratch
exit	Tries to leave (it won't be easy)


Features
Terminal style typewriter output with a command parser
Files that unlock other files as you read them
Random ambient "ghost" messages that grow more frequent and intense
Audio generated live with the Web Audio API (drone, stingers, noise bursts, power-down sound) (and i also did some recording :D)
Screen shake, flicker, night-vision camera overlay and a CRT-style shutdown finale
Fullscreen request on first interaction



kernel_panic.html    # the entire gam - markup, styles, script, embedded image and audio
README.md



Language: vanilla JavaScript (ES2017 async/await), HTML5, CSS3
Audio: Web Audio API for effects, an Audio element for the embedded clip
State: kept in memory only. Refreshing or typing restart resets progress.
Extending it: add content by calling addFile(name, { text, unlocks }), and add commands in handleCommand().


Known Limitations
Requires a user click/keypress before sound plays.
Fullscreen may be blocked by some browsers or embedded frames.
Progress is not saved between sessions.



Credits
Author: Kathirvelan S
