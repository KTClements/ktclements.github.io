[Back to Portfolio](./)

Image Bulk Editor
===============

-   **Class: CSCI 499 - Senior Project Implementation/Defense** 
-   **Grade: B+** 
-   **Language(s): C/C++** 
-   **Source Code Repository:** [features/mastering-markdown](https://github.com/KTClements/CSU-Senior-Project.git)  
    (Please [email me](mailto:ktclements@student.csuniv.edu?subject=GitHub%20Access) to request access.)

## Project description

A cross-platform bulk image editor built with C++ and Qt. Features include auto-white balance, color correction, noise reduction, and batch processing through OpenCV integration. Users can resize, crop, convert formats, and undo/redo operations across multiple images simultaneously. Designed to streamline workflows for photographers, digital marketers, and graphic designers.

## How to compile and run the program

How to compile and run the project.

```bash
qmake
make
./BulkImageTool
```


## UI Design

Launch the app and click Select Folder to load images from a directory, then select any image to preview it below. Use the right panel to apply transformations including rotate (90°, 180°, 270°), flip (horizontal/vertical), auto white balance, and color level adjustment (histogram/gamma), then click Export to save all images in bulk with custom size, format, and quality settings.

![screenshot](images/dummy_thumbnail.jpg)  
Fig 1. The launch screen

![screenshot](images/dummy_thumbnail.jpg)  
Fig 2. Example output after input is processed.

![screenshot](images/dummy_thumbnail.jpg)  
Fig 3. Feedback when an error occurs.

## 3. Additional Considerations

Requires Qt 5 or 6 and a C++17-compatible compiler (g++ or MSVC).
Tested on Windows 10 using Qt Creator and MinGW toolchain.

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

[Back to Portfolio](./)
