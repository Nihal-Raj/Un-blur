# Un-blur
Recover blurred text through Data Science (using [de Bruijn sequence](https://en.wikipedia.org/wiki/De_Bruijn_sequence))

![image](https://github.com/Nihal-Raj/Un-blur/assets/83210067/49ff4a08-72ee-4abb-ae42-ef7a48ba6967)

This algorithm uses the fact that each linear box "filter" processes each block separately. For every block it pixelizes all blocks in the search image to check for direct matches.

After each correct block has no more geometrical match, it will output all the correct blocks directly. 

Tools Required:

- [Python](https://www.python.org/downloads) (Check `Add Python 3.X to PATH)
- pillow library - `pip install pillow` 

How to Run:

- Open command prompt with Administrative Privilege
- Change diretory to a preffered location, say Desktop - `cd %UserProfile%\Desktop` and Create a new folder named "Ub-blur"
- Navigate to the newly created folder - `cd Un-blur`
- Clone the repository via command line - `git clone https://github.com/Nihal-Raj/Un-blur`
- Change directory to the inside folder now -  `cd Un-blur`
- Now unblur the image, (for sample I have already provided blurred images at images\testimages)
- Paste this command:
`depix -p C:\Users\nitu0\Desktop\Depix-main\Depix-main\images\testimages\sublime_screenshot_pixels_gimp.png -s images/searchimages/debruinseq_notepad_Windows10_closeAndSpaced.png -o C:/Users/nitu0/Desktop/output.png`

Explaining the above block of instructions: 
-p tells where the blurred image is located
-s gives the de-Bruijn sequence image for Windows 10 (and 11 also)
-o tells where the output file has to be produced 

Note: In the above case, the output will be at Desktop named "output.png"

That's it!

Thank You
