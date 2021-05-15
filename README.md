# Incogice
An anonymous online counselling web application built using WebRTC and Node.js.
> Know more about WebRTC [here](https://webrtc.org/).<br>
> Know more about Node.js [here](https://nodejs.org/en/).

# How to Run Incogice Locally?
1. Firstly ensure that ```Node.js``` is installed correctly on your local machine, if not then refer <a href="https://nodejs.org/en/download/">this</a>.
1. Clone this repository.
1. After launching an instance of command line in the root folder of this repository, run ``` npm install```. This would install all the required dependencies on your machine.
1. Run  ``` node index.js``` from the commmand line. Now the ```Node.js``` server is running. 
1. From your browser, open ```localhost:8080```. Choose any one counsellor, out the available ones, and click on the corresponding ```Call``` button, allow any kind of access requests for using your camera and microphone (don't worry it is completely safe). 
1. This should redirect you to a call where you should be the only one.
1. Open ```localhost:8080``` again, in a new tab or window. Choose the same counsellor, chosen earlier, and click on the corresponding ```Call``` button, and you should be redirected to the call you joined earlier.
> Now, you should see two videos in each of the two tabs. One video element in each tab displays your local stream and the other video is the remote video streamed via ```WebRTC``` to the second tab. <br>
> You could possibly inspect both the webpages and check that the first webpage would have a console log ```Message from server: Room <room_id> now has 0 client(s)``` where ```<room_id> ``` depends on the counsellor you chose and the second webpage would have a console log ```Message from server: Room <room_id> now has 1 client(s)``` <br>
> This means that initially the room was empty, had 0 clients, when you clicked a ```Call``` button for the first time you joined a room with room-name ```<room_id>``` .
Hence before clicking the ```Call``` button for the second time, there was 1 client already present in the room.  

>Once deployed Incogice would allow users to contact other users using the same mechanism.

Note: You'll need to restart the Node.js server each time you close a client tab or window.
> If you are having odd troubles with caching, try the following:
> 1. Do a hard refresh by holding down ```Ctrl``` key and clicking the Reload button of the browser.
> 1. Restart the browser.
> 1. Run ```npm cache clean``` from the command line.
