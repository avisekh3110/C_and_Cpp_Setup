# C and C++ Setup

Follow the ReadMe to Setup C or C++ Easily.

GO to https://winlibs.com

Win64 (without LLVM/Clang/LLD/LLDB): 7-Zip archive* | Zip archive (LATEST)` 

Extract the file inside and copy the file named "mingW" in C: drive.

Copy the file bin address and paste it -- enviornment variable>>system variable>>path.

paths -- C:\mingw64\bin AND C:\mingw64\x86_64-w64-mingw32\bin

check in cmd --> "g++ --version"

then open vs code you'll find that #include<iostream> in red underline.

click on "bulb button" and click "edit #include path"

{
    "configurations": [
        {
            "name": "Win32",
            "includePath": [
                "C:\\mingw64\\include" --paste the include path here
            ],
            "defines": [
                "_DEBUG",
                "UNICODE",
                "_UNICODE"
            ],
            "compilerPath": "cl.exe",
            "cStandard": "c17",
            "cppStandard": "c++17",
            "intelliSenseMode": "windows-msvc-x64"
        }
    ],
    "version": 4
}

then again go to c/c++ configurations and then change the compiler path to -- 

"C:/mingw64/bin/g++.exe" for c++ AND "C:/mingw64/bin/gcc.exe" for c
