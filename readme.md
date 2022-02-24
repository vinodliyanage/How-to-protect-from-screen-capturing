# How to protect your sensitive data from screen capturing or screen sharing.

Screen sharing! is a word that is often heard these days. Yes, it is important! because of the current situation, but there must be some limit. This article is about how to hide your personal information from screen sharing.

> “They who can give up essential liberty to obtain a little temporary safety deserve neither liberty nor safety.”

                                **― Benjamin Franklin**

## The First Method

Using a dual monitor system. Here you need to run your personal windows apps on a separate monitor. The screen capturing application captures the monitor on which it is running so that the screen of the other monitor is not captured.

## The second method

Run a screen capturing application (e.g., zoom) in a virtual environment (like VirtualBox). Here the application captures the existing environment, so the host environment is not captured.
[VirtualBox](https://www.virtualbox.org/) is an example of a free virtual environment. You can also get the virtual image of windows [here](https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/).

## The third method

In my research on this, I came across the invisiwind application. The tool performs DLL injection to SetWindowDisplayAffinity to WDA_EXCLUDEFROMCAPTUR.
Github: [Invisiwind](https://github.com/radiantly/Invisiwind)

### Running on Windows 11,

This application seems to have some bugs when running on windows 11. I did some testing on early Windows versions. it is working properly on windows 10 or windows 7.
[Please refer here for more analysis and report on this bug](https://docs.microsoft.com/en-us/answers/questions/700122/setwindowdisplayaffinity-on-windows-11.html)
