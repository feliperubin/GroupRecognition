# Authors:
- Felipe Pfeifer Rubin
- Ian Aragon Escobar


# Files:
- 4 testcases, each txt file relates to one mp4 video
- Relatorio.pdf: Describes the work in Portuguese(BR)

# Compile:
- At main.cpp, change the first lines from main() which points to the files .txt
- If you want easily just change to vc[n].filename = argv[n];
- Requires OpenGL (probably >= 2.0)
- gcc  main.cpp vmath.cpp video.cpp -o main 
- Also if not in IDE (e.g. XCode) add -l<library>

# Run:
- ./main
- Space to Pause/Play
* When Paused
	* K to change video
	* Left Arrow go back 1 frame
	* Right Arrow go forth 1 frame
	* Up Arrow go forth 10 frames
	* Down Arrow go back 10 frames
	* [0-9] go to ([0-9]*10)% of the video
	* Esc to exit

# Problems:
* 2 Lines: 
	* 205: glEnable(GL_PROGRAM_POINT_SIZE_EXT);
	* 206: glPointSize(5);
- Comment them (On MacOS HighSierra they work).
- All files are actually Coded in C, only needed thing is to remove the dynamic allocation (malloc/calloc) casting that comes before the function call.

# Example
<img src="/Images/Br1.png" alt="Example" size=/>
