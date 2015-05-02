#Author: Anuj Khandelwal (https://github.com/anujonthemove/)

all: DepthSenseGrabberOpenCV

DepthSenseGrabberOpenCV: DepthSenseGrabberOpenCV.o DepthSenseGrabberCore.o ConversionTools.o
	g++ -o DepthSenseGrabberOpenCV DepthSenseGrabberOpenCV.o DepthSenseGrabberCore.o ConversionTools.o -std=c++11 -lDepthSense -lDepthSensePlugins -lturbojpeg -lusb-1.0 -I/opt/softkinetic/DepthSenseSDK/include -L/opt/softkinetic/DepthSenseSDK/lib `pkg-config --cflags --libs opencv` -I/usr/include/boost -lboost_thread -lboost_system

DepthSenseGrabberOpenCV.o:
	g++ -c DepthSenseGrabberOpenCV.cxx
DepthSenseGrabberCore.o:
	g++ -c DepthSenseGrabberCore.cxx -std=c++11
ConversionTools.o:
	g++ -c ConversionTools.cxx
clean:
	rm -rf *.o DepthSenseGrabberOpenCV