# Small Project Utility

The present bash script help to create `makefile`s for small C/C++ projects. The syntax is the following

```bash
./newproj -compiler name
```
where `-compiler` stands for
* `-gcc` to build a C project with gnu compiler collection
* `-clang` to build a C project with llvm compilers
* `-g++` to build a C++ project with gnu compiler collection
* `-clang++` to build a C++ project wht llvm compilers

The output is a folder named `name` and with the following files and subfolders:
* `src/`: the source files
* `include/`: the headers
* `build/`: the objects (and the building rules, see below)
* `bin/`: the executable
* `makefile`: the makefile (see below)
* `.clang-format`: the configuration file for `clang-format`
