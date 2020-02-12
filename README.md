# ROS cpp format for PAL robotics

This repo contains an auto formatting script for the [ROS C++ Style Guidelines](http://wiki.ros.org/CppStyleGuide) with some
minor adjustments for our style guidelines.

## Clang dependency

This clang format file uses clang-format-4.0

`sudo apt-get install clang-format-4.0`

## Usage with Qt

To set up Qt Creator to use this clang formatting follow the instructions [here](http://doc.qt.io/qtcreator/creator-beautifier.html).

On the **Clang Format** Panel change the **Clang Format command** to 'clang-format-4.0'. After this, choose **Use predefined style: File**.

In /home/USER/ directory clone this repository:

`git clone https://github.com/pal-robotics/roscpp_code_format.git`

and then create a soft link in the /home/USER/ directory pointing to this file and with the same name (.clang-format):

`ln -sf ~/roscpp_code_format/.clang-format`

It is recomended to deactivate the **Enable auto format on file save** option and create a [keyboard shortcut](http://doc.qt.io/qtcreator/creator-keyboard-shortcuts.html) to format the files. To do this, inside QTCreator, go to  Tools – Options – Environment – Keyboard, select ClangFormat / FormatAtCursor, and set the shorcut, e.j. Key Sequence: Ctrl + I 



## Usage with Sublime
Installation Package Control in Sublime:

https://packagecontrol.io/installation

Configuration Clang format in Sublime:

https://github.com/rosshemsley/SublimeClangFormat/blob/master/README.md
