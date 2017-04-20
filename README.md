# Unscentedkalman
This code implements an unscented Kaman filter.


# Instructions to test this code:
# This code was developed and tested using Xcode 8.1 on MacOS Sierra version 10.12.1
# CMAKE version 3.6.1 was used to test for generic compilation. 
# CMakeLists.txt have been created at the top level: Unscentedkalmanproject1
# Another CMakeLists.tx resides in subdirectory /src and another one in subdirectory /data. 
# Two data files are provided with the executable in subdirectory data.
#
# The input data and output data have to be provided as argument to the Main function in the command line
# when executing.
# 
# If the compilation is done using CMAKE and Xcode then you need to configure xcode KalmanProject.xcodeproj
# as follow after CMake has run:
# (1) Edit scheme in Xcode KalmanProject.xcodeproj and add the two arguments filename passed on launch to
# the main.c function
# (2) Tell Xcode where the two input data files are located: 
       go to the "build phases" of the executable and add "copy files"
       select as destination: "resources".
       click on "+"" and select "add other" then browse and select the two input data files

# Change directory to the location of the executable (this path is for compilation using xcode):
# cd UnscentedKalman/build/src/Debug/
# launch the executable
# ./UnscentedKalmanProject sample-laser-radar-measurement-data-1.txt output.txt
