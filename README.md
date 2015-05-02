DepthSenseGrabberOpenCV
=======================

OpenCV based tool for SoftKinetic DepthSense 325 camera.

NOTE
====

This module was taken entirely from https://github.com/ph4m/DepthSenseGrabber

The OpenCV module was isolated for experimenting with DepthSense325 hardware based Senz3D camera.

For any other specific details please refer to the link provided above. 

Build with CMake 2.8 or higher.

Dependencies: DepthSense SDK, boost 1.46.0, OpenCV 2.4.10 (optional)

In detail:
----------

 - DepthSenseGrabberCore is the direct interface to the camera and provides access to the color and depth maps (with or without spatial synchronisation), as well as the acquired confidence map.
 - DepthSenseGrabberOpenCV (requires OpenCV): allows visualization, JPG/PNM export.
 
Modifications:
--------------

- Modified the Cmake file in DepthSenseGrabberOpenCV

Detail:
-------

- Copied all the dependencies from the parent Cmake file (in the main project folder) to the child Cmake file (in the folder DepthSenseGrabberOpenCV). 

- This was done in order to be able to compile the code (in case required) for DepthSenseGrabberOpenCV alone.

Instructions to run:
---------------------

Additions:
----------

- Added optional Makefile
