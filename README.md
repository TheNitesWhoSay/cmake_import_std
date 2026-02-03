# CMake import std
A demonstration of import std in Visual Studios, VS Code, and from command line.

## Setup
- Install and/or update Visual Studios to version 17.14.25 (help -> about should show ``Version 17.14.25 (January 2026)`` or newer)
- In the visual studios installer, modify visual studios 2022, under workloads -> desktop development with C++ -> optional -> ensure you have ``C++ CMake tools for Windows`` installed
- Install and/or update CMake to version 4.2.3 (from powershell, ``cmake --version`` should print ``4.2.3`` or newer*)
- Install and/or update Ninja to version 1.13.2 (from powershell, ``ninja --version`` should print ``1.13.2`` or newer)
- Run ``git clone https://github.com/TheNitesWhoSay/cmake_import_std.git``

\* If you have a newer (or different, but earlier versions may not work at all) version of CMake, make note of what version; then in the following URL: ``https://github.com/Kitware/CMake/blob/v4.2.3/Help/dev/experimental.rst`` replace 4.2.3 with your version, then in the link find ``CMAKE_EXPERIMENTAL_CXX_IMPORT_STD`` and copy the value, and in CMakeLists.txt replace ``d0edc3af-4c50-42ea-a356-e2862fe7a444`` with your copied value.

## Visual Studios
- Right click in the cmake_import_std folder and open with visual studios
- Wait for CMake generation to finish
- Hit f5, the program should compile, run and print ``Hello import std!``

## Visual Studios Code
- Open the cmake_import_std folder in visual studios code
- Hit the build button in the bottom left, select visual studios 2022 x86
- Hit the play button in the bottom left, project should build, run and print ``Hello import std!`` to the terminal

## Powershell
- Open powershell to the cmake_import_std folder
- Run ``mkdir build``, ``cd build``, ``cmake ../``, and finally ``cmake --build .``
- Run ``./Debug/import_std.exe``, it should print ``Hello import std!``

## Results
### Visual Studios
<img width="1966" height="1712" alt="image" src="https://github.com/user-attachments/assets/72a48894-5eb7-44dd-ae3e-d922df141fdc" />

### Visual Studios Code
<img width="2292" height="1329" alt="image" src="https://github.com/user-attachments/assets/fbeb1d3e-bc72-4765-963f-2929771af626" />

### Powershell
<img width="1931" height="1226" alt="image" src="https://github.com/user-attachments/assets/f3833e72-affe-40d0-9a26-650ca892e5d6" />
