# Unofficial collection of SWAT+ code

[![Build by GCC(gfortran) on Linux/macOS](https://github.com/WatershedModels/SWATplus/actions/workflows/cmake_build_gcc.yml/badge.svg)](https://github.com/WatershedModels/SWATplus/actions/workflows/cmake_build_gcc.yml)
[![Build by IntelFortran(ifort) on Linux](https://github.com/WatershedModels/SWATplus/actions/workflows/cmake_build_ifort.yml/badge.svg)](https://github.com/WatershedModels/SWATplus/actions/workflows/cmake_build_ifort.yml)

## 1. About SWAT+ (Soil & Water Assessment Tool Plus)

> SWAT+, a completely revised version of the SWAT model. SWAT+ provides a more flexible spatial representation of interactions and processes within a watershed.

Official site: https://swat.tamu.edu/software/plus/.

Official source code: https://bitbucket.org/blacklandgrasslandmodels/modular_swatplus/src/master/

Latest update: version 60.5.3 with bug fixed, see [this commit](https://github.com/WatershedModels/SWATplus/commit/15c79c2fb25ea99b039497a0f9a19f51c20eeb09).

## 2. About this repository

This is **not** an official repository of SWAT+. 

This repository is an attempt to bring historical releases from official develop team and various enhancement or improvement from scientific community, i.e., the unofficial collection of SWAT+ code. 

CMake build system is used for cross-platform compiling. The [cmake_fortran_template](https://github.com/SethMMorton/cmake_fortran_template) created by [SethMMorton](https://github.com/SethMMorton) is adopted.

Routine testing is done with gfortran compiler on Ubuntu and macOS, and Intel Fortran compiler integrated with MS Visual Studio 2015.

Since I do not have enough test data and the associated SWATplus input files, I have to say, I only compiled various SWATplus versions successfully, but cannot guarantee the validity of running them. So, if you have qualified test data, welcome to contact me (zlj@lreis.ac.cn) for model development and validation and any other purposes.

### 2.1 Branches
+ **develop**: Branch of revised official code. Once a new version of SWATplus source code available, I will create a new branch and merge it to the master branch! Revisions are only made in typos and cross-platform compilations.
+ **master**: Latest official version.
+ **\<MAJOR\>.\<MINOR\>.\<PATCH\>**: SWATplus versions, i.e., `60.5.2`.

### 2.2. Prerequisite

+ CMake2.8+
+ Windows:
  + Microsoft Visual Studio 2010+ and Intel Fortran compiler (ifort) 12.0+
  + or CLion and mingw64 (with gfortran 4.8+)
+ Linux/macOS:
  + GCC (with gfortran installed) 4.8+
  + ifort 12.0+

### 2.3. Compile procedure

+ common commands

  ```shell
  cd <path to SWATplus>
  mkdir build
  cd build
  cmake ..
  make && make install
  ```

# 3. References
+ [Unofficial collection of SWAT code](https://github.com/WatershedModels/SWAT) and 
its [wiki](https://github.com/WatershedModels/SWAT/wiki).