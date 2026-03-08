Readme For Spotify Mood Reccomender

Here is the link to try it yourself https://qratorcode.github.io/Spotify-Web-APP/


  This project is a web application that aligns the user's mood with song recommendations. The recommendations are video game focused, but the algorithm to recommend songs sometimes leads out of that niche.
This was built using the Spotify Web API, built in vanilla HTML, CSS and JavaScript. No frameworks or dependencies were used.
Technical implementation:

-Spotify OAuth 2.0 PKCE flow. This was implemented to generate SHA-256 hashes and base64url encoding for the code challenge and verifier.
-Spotify Web API. A search endpoint was used to query similar tracks to the tags listed in the search parameters.
-Local Storage. This was used to persist the code verifier and access token across the OAuth redirects.
-Dynamic DOM Manipulation. Spotify embed iframes are created and inserted into the results container on each mood selection.
-Animated GIF backgrounds were used to create a more vivid and enjoyable experience for the user.
-This program uses GitHub Pages, so it can be used without a backend. Can be run on PC or iPhone browsers.

User Instructions and Video Examples:

Currently If you want to use this aplication you will have to log in through your spotify account. If that is not something you are comfortable with, I have provided a video demo for both
desktop and mobile.

-Desktop Demo Link https://youtu.be/-QclCTlT-ZI
-Mobile Demo Link https://youtube.com/shorts/kgXl6h5wxXY

Features:

- Can find songs reccomended through catered mood recomendations
- on desktop you can hit the plus button on a song to add it to your liked songs on your spotify account.
- on mobile, you can hit the plus button on a song, which will open the spotify app and give you the option to add it to your liked songs.
- to change the song reccomendations for a specific mood, select a different mood, then go back to the original, and a new song roll will occur.
