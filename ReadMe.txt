This guidance is used to run this liquid tracking project.

1. Compile the project using Cmake. 

2. Open the project, change "Solution Configurations" and "Solution Platforms" into "Release" and "x64", respectively.

3. Open the property menu of this project in "Release | x64" mode to configure the matlab in the following way:
	1) Open the property menu of this project in "Release | x64" mode, select C/C++ ---> General ---> Additional include Directories, and add the following path:
		rootpathofyourmatlab\extern\include
		rootpathofyourmatlab\extern\include\win64

	2) Open the property menu of this project in "Release | x64" mode, select Linker ---> General ---> Additional library Directories, and add the following path:
		rootpathofyourmatlab\extern\lib\win64\microsoft

	3) Open the property menu of this project in "Release | x64" mode, select Linker ---> Input ---> Additional Dependencies, and add the following files:
		libmat.lib
		libmax.lib
		libmex.lib

	4) Minimize your project window and right click "the computer" in the main surface, select 
		Properties --->Advanced System Settings ---> Environment Variables ---> Path ---> Edit
	    then add the new path to your computer:
		rootpathofyourmatlab\bin\win64
  Note the recommended Matlab version is 2020b or other new versions. 

4. Open the project window agaiin and compile this project to generate executable file.

Please download the YOLO files and YOLO deepsort files here, as I can't upload files that exceed 100MB.
https://aaltofi-my.sharepoint.com/:f:/r/personal/yinda_xu_aalto_fi/Documents/Liquid%20tracking%20files?csf=1&web=1&e=RjVKfY
