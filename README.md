# Incogice
An anonymous online counselling web application built using WebRTC.
> Know more about WebRTC [here](https://webrtc.org/).

# How to Run Locally
1. First ensure Node.js is installed on your local machine, if not then  follow <a href="https://nodejs.org/en/download/">this</a>.
1. Clone this repository.
1. After launching an instance of command line in the root folder of this repository. Run ``` npm install```.
1. Run  ``` node index.js``` from the commmand line.
1. From your browser, open ```localhost:8080```.
1. Open ```localhost:8080``` again, in a new tab or window. One video element will display the local stream and the other will show the remote video streamed via ```RTCPeerconnection```.

> You'll need to restart your Node.js server each time you close a client tab or window.
> If you have odd troubles with caching, try the following:
> 1. Do a hard refresh by holding down ```Ctrl``` key and clicking the Reload button of the browser.
> 1. Restart the browser.
> 1. Run ```npm cache clean``` from the command line.
