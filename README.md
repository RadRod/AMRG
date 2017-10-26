Title: Attract Mode romlist generator v2.0b
Date: 10/25/17
Author: Steve Sherrod
URL: http://www.hyperpie.org/

This tool gives the user the ability to create a romlist from favorites tagged via Attract Mode, or by
specifying custom search criteria. This tool can be useful for helping to create collections romlists etc.
This was written as part of Hyperpie V2.

Key features:

- Create a romlist from tagged favorites
- Create a romlist based on user specified search criteria. Any number of strings can be specified (seperate each with comma).
- Ability to search in specific rom information, such as rom name, title, year, or manufacturer.

Misc features:

- Automatically prevents duplicates from being added to output romlist
- User definable romlist path, output directory and filename
- Quick tag search (only searches romlist files that have an accomodating .tag file)

List of available commands:
--help          -h                              Print this help information
--about         -a                              Print the about banner and exit

--tagged        -t      n\a                     Search based on favorites (tagged in Attract Mode)
--search        -s      [string(s)]             Custom search mode (seperate each string with a ',')
--filename      -f      [filename]              Output romlist filename. default: Favorites.txt
--outputdir     -o      [output dir]            Folder to write generated romlist to
--romlistdir    -r      [romlist dir]           AM Romlists location. default: H:\HyperPC\Attract\romlists\
--writemode     -w      [mode]                  Romlist write mode ( append, overwrite). default: append
--param         -p      [param option]          Parameter (token) in romlist to compare to. default: title

Available param (-p) options:   (only applies to custom search mode)
rom     title           year            manufacturer

Command line examples:

AMRG -t
AMRG -t -f faves.txt
AMRG -t -o c:\myromlists -f faves.txt
AMRG -t -r c:\AM\attract\romlists -f faves.txt -o c:\myromlists
AMRG -s mario,luigi,yoshi -p title c:\AM\attract\romlists -f mario.txt -o c:\myromlists
AMRG -s 1982,1983,1986 -p year -f 80s.txt
AMRG -s capcom -p manufacturer c:\AM\attract\romlists -f capcom.txt -o c:\myromlists

Remember that this tool is still in beta, so there may still be a bug or 2.

That's pretty much it! If you have any questions or comments, feel free to contact me on the Hyperpie FB group or forums.
