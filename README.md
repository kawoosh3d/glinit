# GLINIT

Basic OpenGL project

## Setup

Instructions for setting up this project

### GLFW

Install GLFW from https://www.glfw.org/download.html. This project expects GLFW headers to be present at `/usr/local/include/GLFW`.

### Glad

Download Glad related files from https://glad.dav1d.de/. On the website, select

- language: C/C++
- specification: OpenGL
- API - gl: Version 3.3
- Profile: Core
- Options: Tick "Generate a Loader"

Then click the "GENERATE" button to download a zip file. Unzip the file. Then, move the contents of

- the `include` subdirectory (the folders `glad` and `KHR`) into `/usr/local/include` directory.
- the `src` subdirectory (the folder `glad`) into `/usr/local/src` directory

## Build and Run

```
mkdir build
cd build
cmake ..
make
./glinit
```
