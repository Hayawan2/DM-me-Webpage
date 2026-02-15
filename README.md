DM Me Webpage

A sleek, modern web page that allows users to send messages directly to a Discord channel via a secure server. Includes optional name input, live 4K video background, and Discord notifications (pings).

Features

Modern DM card interface with fade-in animation

Optional name input for personalized messages

Live 4K video background for a premium feel

Messages sent via a backend server to keep your Discord webhook secret

Automatic Discord ping to notify the recipient

Fully responsive and works on desktop and mobile

Demo

You can deploy this project on Render or any Node.js hosting platform. Example live demo URL: https://message-button-page.onrender.com

Installation

Clone the repository:

git clone https://github.com/yourusername/message-button-page.git
cd message-button-page


Install dependencies:

npm install


Replace the Discord webhook URL and your user ID in index.js:

const WEBHOOK = 'YOUR_DISCORD_WEBHOOK';
const YOUR_USER_ID = 'YOUR_DISCORD_USER_ID';


Start the server:

npm start

Open index.html in a browser or deploy to a hosting service like Render.

Usage

Users can optionally enter their name. If left blank, messages will appear as from Anonymous.

Messages are sent to Discord via your secure server, keeping your webhook private.

You will get pinged automatically whenever someone sends a message.

File Structure
├─ index.html        # Frontend page with DM card and live background
├─ index.js          # Backend Node.js server handling webhook posts
├─ package.json      # Node.js project configuration
├─ profile.png       # Profile picture displayed on the DM card
├─ background.mp4    # 4K live background video

Dependencies

Express
 – Node.js web framework

CORS
 – To allow cross-origin requests

node-fetch
 – To send requests to Discord

Notes

Make sure your Discord user ID is correct and you’re in the same server as the webhook, otherwise pings will show as Unknown User.

Keep your webhook URL private — do not expose it in frontend code.
