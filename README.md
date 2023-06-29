# The Maze

The Maze is a 3D Maze game that uses ray casting to render a 2D map into a 3D navigable world!

The Maze was written was written in `C` ussing `SDL2` library. Deveploment was performed using `Ubuntu 14.04 LTS` - gcc (Ubuntu 4.8.4-2ubuntu1~14.04) 4.8.4

### About SDL2 

`Simple DirectMedia Layer` is a cross-platform development library designed to provide low level access to audio, keyboard, mouse, joystick, and graphics hardware via `OpenGL` and `Direct3D`. It is used by video playback software, emulators, and popular games including Valve's award winning catalog and many Humble Bundle games.

## Instalation 
```sh
$ git clone
```
## Usage 
* Use up and down arrow keys to move forward and backward (keys `w` and `s` serve the same function)
* Use right and left arrow keys to turn the camera arround (keys `d` and `a` serve the same function)

## Compilation
```sh
$ gcc -Wall -Werror -Wextra -pedantic ./src/*.c -lm -o maze sdl2-config --cflags sdl2-config --libs;
```
## Running
After successfully compiling run the program using following command:

```bash
./maze MAP
```
where ```MAP``` is the name of the file found in the maps folder. You can create other maps and pass them while running program as above. Map files accept only the allowed characters.

## Flowchart
![The Maze Flow Chart](https://i.imgur.com/t0MxNni.png)

## Directories

[`src`]

Contains all the source code files written in C.

[`inc`]

Contains all the header files.

[`maps`]

Contains map data files. This will be used by the program to output the map layout.

[`images`]

Contains image files.

## Images

![image](https://user-images.githubusercontent.com/44834632/138765500-bd3838d0-fe46-4018-87b0-21143fb77e8b.png)

 
## Texture sources

**Weapon**

https://www.seekpng.com/idown/u2w7u2t4i1y3a9y3_call-of-duty-guns-firearms-gun-weapons-coat/

## Contributing

- Read the source files in ```src``` folder and the header files in ```inc``` folder.
- Clone the repo and make a new branch: `$ git checkout -b (name of new branch)`
- Add a feature, fix a bug, or refactor some code :)
- Write/update tests for the changes you made, if necessary.
- Update README.md if necessary.
- Open a Pull Request with a comprehensive description of changes.

### To-Do
- Improved map parser
- Better error handling
- More textures
- Enemies / obstacles / objects
- Maze goal that loads next map
- Rain

### Resources
- [SDL2 API](https://wiki.libsdl.org/CategoryAPI)
- [LazyFoo Beginning Game Programming](http://lazyfoo.net/tutorials/SDL/index.php)
- [Ray-Casting Tutorial For Game Development And Other Purposes by F. Permadi](http://permadi.com/1996/05/ray-casting-tutorial-table-of-contents/)
- [LodeV Raycasting Tutorial](http://lodev.org/cgtutor/raycasting.html)
- [Game Engine Black Book](https://www.amazon.com/Game-Engine-Black-Book-Wolfenstein/dp/1539692876)
