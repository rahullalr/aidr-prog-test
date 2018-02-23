# Web Remote Control

## Scenario

Our customer has a video screen at an exhibition that can be remotely controlled on a local network. In front of the video screen is an tablet device that visitors at the exhibition use to control whats playing.
The customer needs a web application that is hosted on a phone or a tablet and control the machine. They are in a fix and need the app as soon as possible.

## Specifications

Write a simple web application, running on Chrome, Edge, Safari etc. The exhibition visitor should be able to activate three different video sequences through the app.

For handling video sequence selection you should implement a web API with stubbed functions. 
The web API is based on HTTP GET (e.g. Swagger) and implements empty functions (that do not have to communicate with the video screen).
The video screen protocol is based on sequences of UDP packages with customizable text payloads, i.e. commands, and customizable time delay between each message. You do not have to implement this protocol.

The administrator should also be able to change the target host and port for the video screen protocol.

Here is an example for what might be sent if the exhibition visitor initiates a video sequence.

    start video1
    a 500 ms pause
    stop video1
    start video2
    a 1200 ms pause
    start fade
    a 200 ms pause￼
    stop fade
    stop video2

Use the above commands to specify the web API.

## Optional Requirements

* Single-sign-on to the web application. 
* A unit test or two.

## Delivery

A complete Visual Studio project pushed to this repository.

## Time

The app does not have to be perfect nor production ready. Treat it as a first iteration.

With an already set up development environment, the assignment should not take more than 4 hours. Note that this is just an approximation.

## Hints

...￼￼￼