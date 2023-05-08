# Welcome to MovieSync!

A platform to watch movies with your friends! Check out the live project : [http://34.202.237.67:3000/landing](http://34.202.237.67:3001/landing)

## Description

- This platorm supports mp4 files, mpd files (these need to hosted somewhere).
- Plays, pauses, and seeks are synced to all watchers.
- Create separate rooms for for multiple groups.
- We used the following technologies
    - Front End
        - React.js
    - Back End
        - MongoDB
        - Node.js
        - Express.js
    - Testing
        - Selenium
    - Metrics Analysis
        - Python3
- Movie files in mp4 format and chucks created for MPEG_DASH Streaming are stored on AWS S3.
- We use **AWS CloudFront** to stream them seamlessly across the globe.
- We have hosted the server on AWS S3

Architecture

![image](https://user-images.githubusercontent.com/31558571/236909678-9ca4de20-b725-4c10-8b8f-879acccda889.png)

## How to run?

1. Depending on if you want to deploy this project locally or on a server like AWS EC2 you must set your ip in the `/client/src/context/socket.js` If you want to deploy on your local machine, change the server_ip to `localhost. Use the public IP of your server if deploying elsewhere`
2. Clone this repository
3. Navigate to individual folders for client, server, analysis_server and run `npm i` to install npm dependencies
4. Go to analytics_server folder and start it using `node index.js` or `npm run start`
5. Go to server folder and start it using `node server.js`or `npm run start`
6. Then navigate to client and then run `npm run start` to start the client
- You can choose whichever link you want as the url and create a room and then open another instance of the client in the browser and join the room using the room code that is displayed on the screen of the videoplayer.
