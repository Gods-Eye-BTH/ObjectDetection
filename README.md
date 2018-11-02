# ObjectDetection

How to Install:

Step 1: Download the openCV liberary from "https://opencv.org/releases.html"

Step 2: Locate the downloaded liberary.

Step 3: Create a Project and changed the project properties.

Step 3.1: Project Proporties -> Configuration Properties -> VC++ Directories

Step 3.2: Locate both Include Directories and Library Directories

Step 3.3: Locate the new paths for the Include Directories and Library Directories.

Include Directories should look like: C:\Users\Your computer name\Your folder you extracted in\opencv\build\include
Library Directories should look like: C:\Users\Your computer name\Your folder you extracted in\opencv\build\x64\vc15\lib

Step 4: Project Proporties -> Configuration Properties -> Linker

Step 4.1: Change Additional Dependencies to: opencv_world343d.lib

Step 5: You can download the cpp and h files to you Visual Studio and run the program.

IF YOU GET THE ERROR "The code execution cannot proceed becuse opencv_world343d was not found" YOU PUT THE FOLLOWING FILES IN THE SAME FOLDER AS THE PROJECT.

opencv_world343d.lib

opencv_world343d.dll

opencv_world343.dll

opencv_visualisation.exe

opencv_version_win32.exe

opencv_version.exe

opencv_traincascade.exe

opencv_interactive-calibration.exe

opencv_ffmpeg343_64.dll

opencv_createsamples.exe

opencv_annotation.exe

These files are found in: C:\Users\Your computer name\Your folder you extracted in\opencv\build\x64\vc15\bin
---------------------------------------------------------------------------------------------------------------
CODE INFO

There is alot of comments in the code which describes all parts. 

Important parts:

Line 231: capture.open("video-1539252198.mp4"); --> Here you input what should be streamed.

Line 219: bool calibrationMode = true; --> If you want the colormode = false and toolbars to track = ture

Edge map was a test for more options but didnt seem to work.
