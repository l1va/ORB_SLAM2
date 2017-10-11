# ORB-SLAM2

Another fork of [ORB SLAM 2](https://github.com/raulmur/ORB_SLAM2).
All info see there.

Tested with Ubuntu 16.04

Before building orb-slam i was needed:
- install [Glew](https://github.com/nigels-com/glew)
- install [Pangolin](https://github.com/stevenlovegrove/Pangolin). Here i met 
"fatal error: librealsense/rs.hpp: No such file or directory". This
 [fix](https://github.com/stevenlovegrove/Pangolin/pull/190/files) helped. 

Then building orb-slam.

Then building ros example - build_ros.sh

Ok, but when i run it (for example Mono): "error while loading shared libraries: libGLEW.so.2.1: 
cannot open shared object file:" Fixed by (use your version of lib): 
sudo ln -s /usr/lib64/libGLEW.so.1.11 /usr/lib/libGLEW.so.1.11