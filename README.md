thirdparty_submodules
=====================

A repository holding submodules of thirdparty repositories


If you get a warning like:
```
/usr/bin/ld: cannot find -l<some library>
```
Try to add this line to your CMakeLists.txt:
```
link_directories(${CATKIN_DEVEL_PREFIX}/lib)
```
