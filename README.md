# kiss-i3
KISS Linux repo that contains i3-gaps and all of its dependencies.

## Installation
Clone this repo wherever you want (as long as KISS has permission to access it), and add the directory of the repository to the KISS_PATH variable.

### Installing i3-gaps
You also might want to install dmenu, which is in KISS's [Community Repository](www.github.com/kisslinux/community)
```
kiss b i3-gaps
kiss i i3-gaps
```

## Help, yajl won't compile!
If you encounter a problem with yajl not compiling, my current fix is to
```
MAKEFLAGS="" kiss b yajl
kiss i yajl
```
and then install i3 normally.  I am not sure if this is a problem for all computers but it is for me.

## Plans for the future.
I plan to make a package for i3 with rounded corners, if people want that.  Also, I may package up some programs like a compositing manager.  If you want me to add something, please feel free to make a pull request!
