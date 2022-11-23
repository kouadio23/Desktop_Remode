# Overview

Aren't you tired of intructing a person on a call to use their computer? This project gives you a virtual touchpad and a field to type in!

{Provide a description the networking program that you wrote. Describe how to use your software.  If you did Client/Server, then you will need to describe how to start both.}

{Describe your purpose for writing this software.}

{Provide a link to your YouTube demonstration.  It should be a 4-5 minute demo of the software running (you will need to show two pieces of software running and communicating with each other) and a walkthrough of the code.}

[Software Demo Video](http://youtube.link.goes.here)

# Network Communication

{Describe the architecture that you used (client/server or peer-to-peer)}

{Identify if you are using TCP or UDP and what port numbers are used.}

{Identify the format of messages being sent between the client and server or the messages sent between two peers.}


* [Server Script]()
* [Client Script]()
## Usage

* We first need to install the [`pyautogui`](https://pyautogui.readthedocs.io/en/latest/) module to control the cursor and keyboard. Launch <b>Command Prompt</b> or <b>Terminal</b> and type the following:

```
pip install pyautogui
```

* You now need to download [`server.py`]() onto one of the computers and [`client.py`]() to the rest.

* Now run [`server.py`]() on and note the IP address as well as the port that comes as an alert.

* On the other computers, run [`client.py`](). When it asks for the <b>Host IP Address and the Port</b>, type the details that you saw in the alert.

* On the computer running [`server.py`](), you should now see a tkinter window. This window is your virtual touchpad. Click inside the window, and as your cursor moves inside that window, the cursor will move simultaniosly on the client computers!
* You can adjust the window so that the touchpad can reach each end of the client computer. You can use <b>Control + l</b> for left click, <b>Control + r</b> for right click and <b>Control + d</b> for double click. I am working on adding dragging functionality to the touchpad too!

* To type text, click on the <b>'Text'</b> button from the menu of the touchpad. This should bring up a window. Use the text field to enter your text, and click on the <b>'Type Text'</b> button to type the text on the clients, <b>'Delete'</b> for 'backspace' and <b>'Enter'</b> for a new line.


# Development Environment

{Describe the tools that you used to develop the software}

{Describe the programming language that you used and any libraries.}

* Python 3 (I used Python 3.9.0)
* Two or more computers running Windows / macOS / Linux
* All computers need to be connected to the same network

# Useful Websites

{Make a list of websites that you found helpful in this project}
* [Web Site Name](http://url.link.goes.here)
* [Web Site Name](http://url.link.goes.here)

# Future Work

{Make a list of things that you need to fix, improve, and add in the future.}
* Item 1
* Item 2
* Item 3

1. <h3><b>Lag in the movement of the cursor</b></h3>This happens only if your network connection is unstable or slow.

2. <h3><b>The touchpad takes my complete screen, but it still does not access the clients complete screen</b></h3>Try changing the '2' of line 40 in server.py to a higher number, such as 3 or 4.

In the case that you found any other bugs in the code, create an issue or send an email to [kouaokouadio@gmail.com](mailto:kouaokouadio@gmail.com) and I will fix it as soon as possible.