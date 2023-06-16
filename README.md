# Un-blur
Recover blurred text through Data Science (using [de Bruijn sequence](https://en.wikipedia.org/wiki/De_Bruijn_sequence))

![image](https://github.com/Nihal-Raj/Un-blur/assets/83210067/49ff4a08-72ee-4abb-ae42-ef7a48ba6967)

This algorithm uses the fact that each linear box "filter" processes each block separately. For every block it pixelizes all blocks in the search image to check for direct matches.

After each correct block has no more geometrical match, it will output all the correct blocks directly. 
