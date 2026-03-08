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



 I initially chose this assignment because I needed something I could complete in a day that still provided enough of a challenge. Overall I am really glad I took on this project, it has helped a lot with becoming more familiar with API integration.
My main errors were 403 errors from Spotify's dev mode blocking playlist API access. Another problem was that my search tags were getting hijacked by Spotify's algorithm. For example, searching "Disco Elysium OST" would return songs with "disco" in the title instead of the actual game soundtrack. Another bug I encountered was that the authorization code Spotify returns in the URL was being reused on every page reload, causing authentication to fail after the first login. I fixed this using window.history.replaceState to clear the code from the URL immediately after it was used.
I chose the OAuth 2.0 PKCE flow specifically because it is designed for client-side apps with no backend required. This enabled me to work faster as I am a more frontend focused programmer, and makes it easier for new users to access since all they need is a link. Originally I was using playlist IDs as it allowed for exact playlist customization, but I had to pivot to keyword search due to the 403 dev mode restrictions. Lastly I used vanilla JavaScript over a framework because it provided simplicity and made it easy to deploy as a static site.





