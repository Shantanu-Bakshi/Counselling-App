# Incogice
An anonymous online counselling web application built using WebRTC.
> Know more about WebRTC [here](https://webrtc.org/).

# How to Run Incogice Locally?
1. Firstly ensure that ```Node.js``` is installed correctly on your local machine, if not then refer <a href="https://nodejs.org/en/download/">this</a>.
1. Clone this repository.
1. After launching an instance of command line in the root folder of this repository, run ``` npm install```. This would install all the required dependencies on your machine.
1. Run  ``` node index.js``` from the commmand line. Now the ```Node.js``` server is running. 
1. From your browser, open ```localhost:8080```. Choose any one counsellor, out the available ones, and click on the corresponding ```Call``` button, allow any kind of access requests for using your camera and microphone (don't worry it is completely safe). This should redirect you to a call with the chosen counsellor (but you are the only one till now).
1. Open ```localhost:8080``` again, in a new tab or window. Choose the same counsellor, as the previous step, and click on the ```Call``` button, and you should be redirected to the call you joined in the previous step.
> Now, you should see two videos in each of the two tabs. One video element in each tab displays your local stream and the other video is the remote video streamed via ```WebRTC``` to the second tab.

Note: You'll need to restart the Node.js server each time you close a client tab or window.
> If you are having odd troubles with caching, try the following:
> 1. Do a hard refresh by holding down ```Ctrl``` key and clicking the Reload button of the browser.
> 1. Restart the browser.
> 1. Run ```npm cache clean``` from the command line.
