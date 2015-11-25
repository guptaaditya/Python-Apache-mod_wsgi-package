# Python-Apache-mod_wsgi-package
1) Prepare system.
	a) go to control panel->Programs. Check if there are any microsoft visual c++ redistributables. If there are any above 2010 uninstall all of them.
	b) If python version above 3.3.0 is installed uninstall it.

2) Installation steps.
	a) Extract package in C directory. Strictly follow the instructions or you will run into configuration issues.
	b) There now exists a folder in C directory called pythonsetupweb consisting of Apache2, and this document, .msi and .exe
	c) Run vc_redistr2010.exe
	d) Run vc_redistr2015.exe
	f) Eun python.msi and let the installer install it in default path C:\Python33
	g) Open Apache2/bin folder. In address bar type cmd and press enter. Or other wise open cmd and navigate to C:\pythonsetupweb\Apache2\bin
	h) Run httpd.exe on cmd. If it runs without error, open browser and type localhost:81/test.py.
	i) Cheers when you see 'hello world'.

	j) This step is optional. If you want to install apache as service, then close the command prompt window, and run installservice.bat file present inside C:\pythonsetupweb\Apache2 folder
