# Image-Manipulation

## Feature One
Displays the bmp file's information such as width, lenght, bpp, padding and data offset.

### Compilation
```bash
gcc bmp_info.c helper_functions.c imageManipulation.c -o bmp_info 
```

### Running
``` bash
make test
```
or 
``` bash
./bmp_info dog.bmp 
```

## Feature Two
Resizes the pixel data of an image by a scaling factor given as an argument.

### Compilation
``` bash
 gcc bmp_scale.c helper_functions.c imageManipulation.c -o bmp_scale
 ```
 
 ### Running
 ``` bash
  ./bmp_scale dog.bmp dog_scaled.bmp 0.5
  ```
  
  ## Feature Three
  Open two BMP files, and combine their contents by laying one over top of the other,
respecting that the “alpha” channel of the foreground image indicates transparency. Alpha values of 0
mean the background image should show through.

### Compilation
``` bash
 gcc bmp_collage.c helper_functions.c A3_solution.c -o bmp_collage
```

### Running
``` bash
 ./bmp_collage robots.bmp rabbit.bmp robots_with_one_ear.bmp 80 770 1.0
```
``` bash
 ./bmp_collage robots_with_one_ear.bmp dog.bmp robots_with_both_ears.bmp 190 205 0.5
 ```
 
 
