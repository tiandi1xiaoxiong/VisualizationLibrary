# Visualization Library

<img src="http://visualizationlibrary.org/docs/2.0/gallery/tess04.jpg" width=128> <img src="http://visualizationlibrary.org/docs/2.0/pics/pagGuideStereo_1.jpg" width=128> <img src="http://visualizationlibrary.org/docs/2.0/gallery/raycast01.jpg" width=128> <img src="http://visualizationlibrary.org/docs/2.0/gallery/mandel04.jpg" width=128 height=128>

<img src="http://visualizationlibrary.org/docs/2.0/gallery/mol02.jpg" width=128> <img src="http://visualizationlibrary.org/docs/2.0/gallery/bezier01.jpg" width=128> <img src="http://visualizationlibrary.org/docs/2.0/gallery/edge04.jpg" width=128> <img src="http://visualizationlibrary.org/docs/2.0/gallery/extrude02.jpg" width=128>

<img src="http://visualizationlibrary.org/docs/2.0/gallery/glsl16.jpg" width=128> <img src="http://visualizationlibrary.org/docs/2.0/gallery/glsl07.jpg" width=128> <img src="http://visualizationlibrary.org/docs/2.0/gallery/raycast04.jpg" width=128> <img src="http://visualizationlibrary.org/docs/2.0/gallery/marching-plot.jpg" width=128>

[More Pictures](http://VisualizationLibrary.org/gallery)

## About

Visualization Library is a C++ middleware for high-performance 2D and 3D graphics applications based on the industry standard OpenGL 1.x-4.x, designed to develop portable applications for the Windows, Linux and Mac OS X operating systems.

## Compilation and Installation

### Windows CLI

- Install CMake 3.x: https://cmake.org/download/
- Install Doxygen 1.8.x: http://www.doxygen.nl/download.html (optional to build the docs, remove `-DVL_BUILD_DOCS=ON` if not interested)
- Install Qt5 (optional, to run the Qt5 GUI bindings, remove `-DVL_GUI_QT5_SUPPORT=ON` `-DVL_GUI_QT5_EXAMPLES=ON` if not interested)

Example to build and install a `Debug` build of VL and run the `vlQt5_tests.exe glsl` test:

```
cd C:\
git clone git@github.com:MicBosi/VisualizationLibrary.git
cd VisualizationLibrary
mkdir _BUILD
mkdir _INSTALL
cd _BUILD
cmake .. -G "Visual Studio 16 2019" -DVL_GUI_WIN32_SUPPORT=ON -DVL_GUI_WIN32_EXAMPLES=ON -DVL_GUI_QT5_SUPPORT=ON -DVL_GUI_QT5_EXAMPLES=ON -DVL_INSTALL_DATA=ON -DVL_BUILD_DOCS=ON -DCMAKE_INSTALL_PREFIX='C:\VisualizationLibrary\_INSTALL\'
cmake --build . --config Debug --target INSTALL
cmake --build . --config Debug --target Docs
set PATH=%PATH%;C:\VisualizationLibrary\_INSTALL\bin
set VL_DATA_PATH=C:\VisualizationLibrary\_INSTALL\data
vlQt5_tests.exe glsl
```

### Windows, Linux, Mac

Follow the instructions here: http://visualizationlibrary.org/docs/2.0/html/pag_install.html

## Licensing

Visualization Library is released under the OSI approved Simplified BSD License ([LICENSE.md](LICENSE.md)).

## Resources

* Official website and documentation: [VisualizationLibrary.org](http://VisualizationLibrary.org)
  
* Support and contribution:
    * [Visualization Library Google group](https://groups.google.com/forum/#!forum/visualization-library).
    * [Issue tracker on GitHub](https://github.com/MicBosi/VisualizationLibrary/issues).
    * Send your patches via [GitHub pull request](https://help.github.com/articles/using-pull-requests/).

* Releases: [github.com/MicBosi/VisualizationLibrary/releases](https://github.com/MicBosi/VisualizationLibrary/releases)

* Sources: [github.com/MicBosi/VisualizationLibrary](https://github.com/MicBosi/VisualizationLibrary)

* Download page: [VisualizationLibrary.org/download](http://VisualizationLibrary.org/download)

* Contacts: 
    * michele *at* visualizationlibrary *dot* org
    * [twitter.com/VizLibrary](https://twitter.com/VizLibrary)
    * [michelebosi.com](https://michelebosi.com)

Happy coding :)
