# Fish-eye-Image-Correction-Code

## The basic features of the project:

You can use this program to carry out basic experiments for circular fisheye images:

* Circular Area Parameters Extration.
* Image Correction.
* Stitching corrected images into a panorama.
* navigate the produced panorama.

User experience is not so good, it only has basic functions.

## The demo video play

[![demo vide](https://img.youtube.com/vi/4rHV4EqkvDQ/0.jpg)](https://www.youtube.com/watch?v=4rHV4EqkvDQ)

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

**The project is in developing, so it may be updated sometime when I feel there should be added something. If you have any question, please connect author or fire an issue on this repo. I will be very happy if I know you are interested in this project. ;-D**


## The project directory tree struct is as follow:

```bash
.
├── ImagesForTest
│   ├── 1
│   ├── 2
│   ├── 3
│   ├── 4
│   ├── 5
│   ├── 6
│   ├── 7
│   ├── 8
│   ├── 9
│   ├── other
│   └── valid_params.txt
├── README.md
├── build.sh
├── opencv
│   ├── contrib
│   ├── extra
│   └── main
├── paper
│   ├── 毕业答辩.pptx
│   ├── 处理过程演示视频.mp4
│   ├── 单幅圆形鱼眼图像的校正.pdf
│   └── 鱼眼成像全景漫游系统的研究.docx
├── product
├── program
│   ├── corrector.cpp
│   ├── corrector.h
│   ├── findCircleParameter.cpp
│   ├── findCircleParameter.h
│   ├── globalInclude.h
│   ├── imagesStitcher.cpp
│   ├── imagesStitcher.h
│   ├── main.cpp
│   ├── tools.cpp
│   ├── tools.h
│   ├── viewer.cpp
│   └── viewer.h
├── resources
│   ├── 1.JPG
│   ├── 2.JPG
│   ├── 3.JPG
│   ├── 4.JPG
│   ├── corrected0.jpg
│   ├── corrected1.jpg
│   ├── corrected2.jpg
│   ├── corrected3.jpg
│   ├── navigate.png
│   └── panorama.jpg
├── run.sh
└── setup-vsc.sh

20 directories, 31 files
```
