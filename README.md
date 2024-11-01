# Fish-eye-Image-Correction-Code

## The basic features of the project:

You can use this program to carry out basic experiments for circular fisheye images:

* Circular Area Parameters Extration.
* Image Correction.
* Stitching corrected images into a panorama.
* navigate the produced panorama.

User experience is not so good, it only has basic functions.

## The demo video play

Link For the demo Video:

https://www.youtube.com/watch?v=BQV-URN5nwE&ab_channel=kaosainakbar

## How to use this project

1. pre-requirements: 
    - required: 
        - [**install clang++ compiler**](https://clang.llvm.org/cxx_status.html)
            - MacOS: you can install Xcode to get the clang++ available automaticlly
            - Linux: install clang is not so diffcult, do some research yourself.
            ```bash
            $ sudo apt-get install -y clang git cmake
            ```
        - [**install cmake build tool**](https://cmake.org/download/)
    - optional:
        - [**visual studio code**](https://code.visualstudio.com/)

2. clone repo into you local disk as follow: 

    ```bash
    git clone --recurse-submodules https://github.com/wangzhizhou/Fish-eye-Image-Correction-Code.git
    ```
    this repo have three opencv source repos as submoudle, 
    fetch opencv repos may cost some time, 
    if you live in chinese mainland, `github.com` maybe blocked, 
    please notice these problem
3. change working directory into local repo, build successfully and run program:

    ```bash
    cd Fish-eye-Image-Correction-Code/ && ./build.sh && ./run.sh
    ```

    `run.sh` script use the `ImagesForTest/1/*jpg` images as demonstration.

### Sample Processing

OK! Probably like this. Here is a sample processing.

#### The original images
![image1](https://github.com/wangzhizhou/Fish-eye-Image-Correction-Code/blob/master/resources/1.JPG)
![image2](https://github.com/wangzhizhou/Fish-eye-Image-Correction-Code/blob/master/resources/2.JPG)
![image3](https://github.com/wangzhizhou/Fish-eye-Image-Correction-Code/blob/master/resources/3.JPG)
![image4](https://github.com/wangzhizhou/Fish-eye-Image-Correction-Code/blob/master/resources/4.JPG)

#### The corrected images
![corrected1](https://github.com/wangzhizhou/Fish-eye-Image-Correction-Code/blob/master/resources/corrected0.jpg)
![corrected2](https://github.com/wangzhizhou/Fish-eye-Image-Correction-Code/blob/master/resources/corrected1.jpg)
![corrected3](https://github.com/wangzhizhou/Fish-eye-Image-Correction-Code/blob/master/resources/corrected2.jpg)
![corrected4](https://github.com/wangzhizhou/Fish-eye-Image-Correction-Code/blob/master/resources/corrected3.jpg)

#### The stitched panorama
![panorama](https://github.com/wangzhizhou/Fish-eye-Image-Correction-Code/blob/master/resources/panorama.jpg)

#### navigate the panorama
![navigate](https://github.com/wangzhizhou/Fish-eye-Image-Correction-Code/blob/master/resources/navigate.png)

