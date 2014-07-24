Using cURL
====

cURL
You can easily interact with the M2X API using cURL, a powerful command-line tool for making HTTP calls.
** Pre-requisites: Windows 7 or later, or Mac OS X 10.7 or later**

### Downloading + installing cURL on Windows
***(cURL is already installed on Mac computers)***
Use the following steps to install curl:
Open http://curl.haxx.se/dlwiz?type=bin in a browser.
Select your operating system in the dropdown box: either Windows /Win32 or Win 64. Click Select!
For Win 32, choose whether you will use curl in a Windows Command Prompt (Generic) or in a Cygwin terminal (cygwin). For Win 64, choose whether you will use curl in a Windows Command Prompt (Generic) or MinGW (MinGW64). ClickSelect!
If required, choose your Windows operating system. Finish.
Click Download for the version which has SSL enabled.
Choose a version with support for SSL.
Open the downloaded zip file. Extract the files to an easy-to-find place, such as C:\Program Files.
Testing curl on Windows
Open up the Windows Command Prompt terminal. (From the Start menu, click Run, then type cmd.)
Set the path to include the directory where you put curl.exe. For example, if you put it in C:\Program Files\curl, then you would type the following command:
set path=%path%;"c:\Program Files\curl"
Type curl.
You should see the following message:
curl: try 'curl –help' or 'curl –message' for more information
This means that curl is installed and the path is correct.
Type:
curl https://api-m2x.att.com/v1
You should see JSON returned:
{
"message":"You must provide a valid API key in the X-M2X-KEY header"
}

Testing curl on Mac OS X
Open up a Terminal Window (Terminal can be launched from Spotlight, the Dock at the bottom of the screen or even the Applications folder)
Type curl.
You should see the following message:
curl: try 'curl –help' or 'curl –message' for more information
This means that curl is installed and the path is correct.
Type:
curl https://api-m2x.att.com/v1
You should see JSON returned:
{
"message":"You must provide a valid API key in the X-M2X-KEY header"
}