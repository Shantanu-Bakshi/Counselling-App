# Incogice
An anonymuous online counselling web application employing WebRTC.
> Know more about WebRTC [here](https://webrtc.org/).

# How to Run Locally
1. First ensure Node.js is installed on your local machine, if not then <a href="https://nodejs.org/en/download/"> Download it from here </a>.

1. Download this repository

1. After launching an instance of the command prompt in the root folder of this repository. Run ``` npm install```.
1. Run  ``` node index.js``` from the commmand prompt.
1. From your browser, open localhost:8080.
1. Open localhost:8080 again, in a new tab or window. One video element will display the local stream from ```getUserMedia()``` and the other will show the ‘remote' video streamed via RTCPeerconnection.

> You'll need to restart your Node.js server each time you close a client tab or window.
