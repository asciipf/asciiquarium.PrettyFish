# asciiquarium.PrettyFish
------------

+ The sole aim of asciiquarium.PrettyFish is simply to make Kirk Baucom's original asciiquarium just a little prettier.
    + It slightly alters the possibilities for fish speed, which may make fish movement look less 'jerky'.
    + It slightly changes the bubble pattern and rate.
    + It makes the fish more 'slippery' by replacing spaces OUTSIDE the outline of the fish proper with a '?', which instructs the Term::Animation program to render those spaces as transparent (rather than solid black). Result: fish look more like they're sliding past one another.
    + It adds the color white to the possible colors for the fish body, dorsal fin, etc. (Previously only the eyes could be white).
    + It substantially modifies one original fish.
    + It deems one original fish so 'un-pretty' as to be unsalvageable, and eliminates it.
    + It adds, and then modifies, four (unsourced) new fish.
    + It adds (these are original compositions) a turtle, a 'fan fish', and a scuba diver.
    + It triples the incidence of all the 'regular' fish so that the scuba diver and the 'fan fish' don't appear too often.

For full screen viewing, try something like this:

urxvt -fn "xft:DejaVu Sans Mono:pixelsize=50" -geometry 1000x1000 -e /bin/sh -c "asciiquarium.PrettyFish"

    + DejaVu Sans Mono -- or another UTF mono font you like
    + adjust 'pixelsize' to your taste and for your screen
    + '-geometry 1000x1000' will expand the terminal
        as large as possible for your screen
    
------------
                              Asciiquarium v1.1
                    by Kirk Baucom <kbaucom@schizoid.com>
                          http://www.robobunny.com

Asciiquarium is an aquarium/sea animation in ASCII art.

Installation
------------

Asciiquarium is a single perl script, so all you have to do is make sure
it's executable and put it somewhere convenient, like /usr/local/bin or
/usr/local/games.

  Ubuntu
  ------

  Out-of-the-box ubuntu doesn't satisfy the Requirements below, so
  here's how to get them:
  1) Get perl's curses package which is available from apt:
       sudo apt-get install libcurses-perl
  2) Run
       cpan
     at the shell.  Agree to the defaults for everything.
     To leave cpan, type 
       quit
  3) Type
    sudo cpan Term::Animation

Requirements
------------

You must have the Term::Animation module, which you can get from
http://www.cpan.org. The Term::Animation module also requires the Curses
module, which you can also get from CPAN. This program will only run on
platforms that have a Curses library (so it won't work on Windows, but
you might get it to run under cygwin).

Usage
-----

Command line arguments:
	-c	"classic" mode, only show species from Asciiquarium 1.0

While running:
	q	quit
	r	redraw (will recreate all entities)
	p	toggle pause

Contributors
------------

New fish species backported from the Android live wallpaper and
other minor improvements by Claudio Matsuoka.

Pretty much all of the ASCII art was done by Joan Stark:
http://www.geocities.com/SoHo/7373/

Anything that she didn't do, I don't have a source for.


