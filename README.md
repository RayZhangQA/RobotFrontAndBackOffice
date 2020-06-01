# RobotFrontAndBackOffice

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.


### 1. Setup

-	Download Python & Install Python & Add the path to System Variables 
-	Check if Python is installed properly in your system

		python --version
		pip --version

-	Install and uninstall Selenium

		pip install selenium
		pip uninstall selenium

-	Install robot framework	

		pip install robotframework
		pip install --upgrade robotframework
		pip install robotframework==2.9.2
		pip install –no-cache-dir robotframework
		pip uninstall robotframework

-	Install Robotframework Selenium Library	

		pip install robotframework-seleniumlibrary
		pip uninstall robotframework-seleniumlibrary
		pip list
		pip show robotframework
		pip check robotframework

-	Download and Install Eclipse IDE
-	Install RED-Robot Editor from Eclipse Marketplace

		Eclipse>>Help>>Eclipse Marketplace>>Search for RED Robot Editor>>Install and Restart Eclipse
	RED requires python interpreter with robot framework installed in your system.

		Eclipse>>Windows>>Preferences>>Robot Framework>>Installed frameworks

	You should see the python which automatically created.
	In case you have multiple version of Python you need select the correct one to use

-	Install CodeMix3 for Python Pack from Eclipse Marketplace
-	Copy the Chromedriver.exe to ../Python37/Scripts/ Folder.



### 2.	Executing the tests with the Tags

		robot --include=sanity test\TaggingTest.robot
		robot --include=regression test\TaggingTest.robot
		robot -i sanity -i regression test\TaggingTest.robot
		robot -e regression test\TaggingTest.robot

### 3.	Executing Test Suites
•	Appraoch1 – Specify Folder

		cd C:\User\Administrator\eclipse-workspace\RobotPOM
		robot TestCases\
•	Appraoch2 – Using Regular Expression

		cd C:\User\Administrator\eclipse-workspace\RobotPOM
		robot TestCases\*.robot
		robot TestCases\*Reg.robot

### 4.	Executing Tests Parallelly using robotframework-pabot
•	Install robotframework-pabot

		pip install -U robotframework-pabot

•	Run Test Parallelly 

		cd C:\User\Administrator\eclipse-workspace\RobotPOM
		pabot --processes 2 TestCases\*.robot



### Documentation

More reading available [here](https://github.com/ShawONEX/qa-automation/tree/master/WebDriver/docs)
