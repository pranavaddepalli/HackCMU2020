## Inspiration
Due to the COVID-19 pandemic, people were forced to abandon plans of in-person gatherings in favor of meeting up with friends on virtual platforms. One frequently utilized social platform is Discord, which allows people to come together and talk when not physically together. However, such virtual platforms have their limitations: Discord does not allow for the streaming of perfectly synchronous video, making it impossible to watch and enjoy youtube videos with friends as lag causes people's videos to desynchronize.

## What it does
Spectre, a synchronous video-watching platform for you and your friends that can be initiated in a discord server with a simple command: !watch [youtube link]. The bot will reply with a message containing a link to the room. You and anyone who wishes to watch with you can click on the link to join the room. The homepage will require you to enter a username before entering the room itself, where you can then watch the linked video with friends. Inside the video room, there are features available to enhance your viewing experience, including changing host permissions or adding videos to the queue. The chatroom is linked with Discord so that messages sent in discord will show up in the chatroom.

## Our Stack
The languages we used to build this project were Python, JavaScript, and markup language (HTML/CSS). The Discord bot was built using Python and the discord.py Discord API. The spectre platform backend was built in JavaScript, using an Express.js server, Node.js, and WebSocket. The front end of the website was designed using HTML and CSS.

## How we built it
Our Discord bot implemented the Discord API in order to interact with users. It works in conjunction to the server backend, and communicates to it via a RESTful API. The backend server uses websockets to synchronize video playing between devices, and interacts with the YouTube Data API v3 for video playback from YouTube. The framework for the front end, the implementation of the websocket, and the chat backend was adapted from Vynchronize. However, with the addition of the new API and with the connection of the Discord bot to our website, most existing features were incompatible, so we had to do a complete rehaul. We also improved the appearance and ease of use of the front end. The website was designed with HTML and CSS, with JQuery and AJAX for server communication.

Vynchronize is licensed under the MIT License.

## Challenges we ran into
When we initially had an idea, we realized that it would be impossible to learn how to implement a video player that would synchronize across users' screens in 24 hours, so we were forced to rely on a pre-existing framework. Another challenge was that the framework had to be adjusted quite a lot to suit our needs, which was to communicate with a discord bot. 

## Accomplishments that we're proud of
We are proud of being able to adapt to a new framework and a programming language we haven't worked with before, in addition to learning using an existing framework to add an API. We also intially struggled a bit with displaying our product before figuring out how to deploy to Heroku.

## What we learned
Through the production of this project, we gained a lot of experience using Express.js and Node.js and websockets for the backend. We learned more about the Discord API and creating a functioning bot. Through creating the frontend of the webpage such that it was compatible with the framework, we learned Boostrap and embedded CSS.

## What's next for Spectre
For the Discord bot, we want to implement more features that will make going between Discord and Spectre easier. In addition, we hope to add more interesting features to the website that will enhance the video watching experience, as well as add support for other widely-used video players, and potentially even include support for popular apps like TikTok. We would also like to improve the accessibility of the site, such as by supporting high contrast or light mode and much more alt text. 
