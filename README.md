Information for installing OpenCV on linux (e.g., amazon aws):

from http://docs.opencv.org/doc/tutorials/introduction/linux_install/linux_install.html#linux-installation

> Create a temporary directory, which we denote as <cmake_binary_dir>, where you want to put the generated Makefiles, project files as well the object files and output binaries.
>
> Enter the <cmake_binary_dir> and type
>
> cmake [<some optional parameters>] <path to the OpenCV source directory>
> For example
>
> cd ~/opencv
> mkdir release
> cd release
> cmake -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/usr/local ..
> Enter the created temporary directory (<cmake_binary_dir>) and proceed with:
>
> make
> sudo make install


