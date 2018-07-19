# VGAlizator

 Little python script to transform .ppm files into something possible for program intended to run in VGA to read, it works by transforming the colors in the file into indices in a pallette (be careful of the 256 color limit in vga), creating a .pgm file with each pixel value being the index of a color, and creating a .plt file with similar structure to .pgm and .ppm, with the indices and color values, properly limited between 0 and 63.
 
 Arguments: python vgalizator.py ppmin startIndex endIndex filesOut
 
 Structure of .plt files
 
 The .plt files follow the following structure:
 
 index r g b\n
 
 index r g b\n
 
 ...
 
 Example:
 
 0 20 30 63
 
 3 30 10 50
 
 2 10 30 50
