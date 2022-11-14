# Qt LGPL v3 license used by Yealink Meeting/UME
Yealink Meeting/UME used modified Qt libs for specified functions and show the changes in this github path:  
[https://github.com/Yealink-PC-App/qtbase]  
you can check changes from the link below:  
[https://github.com/Yealink-PC-App/qtbase/commit/6bf304db8d7dc13ff5a7f398f37ee0e34e58a16c]  

# How to replace modified qt lib into Yealink Meeting/UME
1. pull modified qt code from project https://github.com/Yealink-PC-App/qtbase/
2. run cmd below
```
configure -prefix d:\xxxx\  -debug-and-release -confirm-license -opensource -shared -force-debug-info -opengl dynamic -platform win32-msvc2017 -c++std c++11 -nomake tests -nomake examples  -skip qtwebengine -mp
```
 - "d:\xxxx\" means compile target path, you can replace any other available path.
 - "-platform win32-msvc2017" means compiler, you can replace any other available compiler.
 - other configs are all not fixed, you can adjust if need

3. compile qt like official ways
4. copy qt libs into Yealink Meeting/UME install path and replace current libs

