[ >>> 中文版](README_ch.md)

The QCefWidget project provide a widget that is used to view webpage. 

Support:

✅ Supports both CEF OSR and non-OSR mode;
   
✅ Show background transparent webpage in irregularity window;

✅ Javascript and Qt interaction;

✅ OpenGL graphics acceleration;

✅ Third-party input method software;

✅ Perfect exit app without any CEF assert/exception in debug/release mode;

✅ Separate CEF rendering process and plugin process;

✅ Support Adobe Flash without any warnning, eg "Control-click to run Adobe Flash Player".

✅ Drag/Drop frameless window like Electron throught setting CSS property.

---


## Build Instruction

1. Download and install [CMake](https://cmake.org/)

2. Download and install Qt SDK from [Qt Downloads](https://download.qt.io/archive/qt/)

3. Download CEF binary distribution [Chromium Embedded Framework (CEF) Automated Builds](https://cef-builds.spotifycdn.com/index.html) and extract it to ***dep*** directory, for example:
    ```
    root
    ├─dep
    │  └─cef_binary_80.1.15+g7b802c9+chromium-80.0.3987.163_windows32
    ├─src
    └─test
    ```

4. Update the [config.cmake](config.cmake) to set the required build configurations

5. Using CMake to build the project, for example:
    ``` bat
    mkdir build && cd build
    cmake .. && cmake --build .
    ```
    
## Test
QCefWidget has been tested with follow Qt and CEF version:

|Qt Version|CEF Version|Pass|
|---|---|---|
|5.12.10|3.3626.1895|✅|
|5.14.2|3.3626.1895|✅|

## Usage
QCefWidgetTest is a perfect demo about how to use QCefWidget in `test` folder.

![screenshot1 on windows](test/Screenshot/screenshot1.png)

![screenshot2 on windows](test/Screenshot/screenshot2.png)
