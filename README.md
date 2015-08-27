Information for installing OpenCV on linux (e.g., amazon aws):

Download the package from http://opencv.org/downloads.html.  

Installation instructions are here:
http://docs.opencv.org/doc/tutorials/introduction/linux_install/linux_install.html#linux-installation

First, install required packages:
>     [compiler] sudo apt-get install build-essential
>     [required] sudo apt-get install cmake git libgtk2.0-dev pkg-config libavcodec-dev libavformat-dev libswscale-dev
>     [optional] sudo apt-get install python-dev python-numpy libtbb2 libtbb-dev libjpeg-dev libpng-dev libtiff-dev libjasper-dev libdc1394-22-dev

Then:
>     Create a temporary directory, which we denote as <cmake_binary_dir>, where you want to put the generated Makefiles, project files as well the object files and output binaries.
>
>     Enter the <cmake_binary_dir> and type
>
>     cmake [<some optional parameters>] <path to the OpenCV source directory>
>     For example
>
>     cd ~/opencv
>     mkdir release
>     cd release
>     cmake -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/usr/local ..
>     Enter the created temporary directory (<cmake_binary_dir>) and proceed with:
>
>     make
>     sudo make install

The videos come from https://www.youtube.com/watch?v=8MmC8HIC44o
Which I found by searching for "clips of tennis serves with speed"

I also installed avconv, which you get from libav-tools, which you can also get with ffmpeg
>    sudo apt-get install ffmpeg
