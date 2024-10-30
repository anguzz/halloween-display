This web page contains an IFrame pointing to a youtube playlist comprised of scary or halloween related videos, to be used as a background for displays for halloween parties, below are some instructions on how to make the most of it with a mini desktop running windows. The reason I created an IFrame to serve this instead of playing the playlist on the display is because you get more control over certain properties through youtube embedded Iframes. My use case is it's going to be used on a small mini pc at a halloween party as a backdrop with a projector


- Enable auto-login on windows
- On windows desktop create a new shortcut
- use the following, which will open it up in fullscreen kiosk mode 
"C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" --kiosk "https://h.angs.dev/"
- Now use windows+R to run shell:startup
- Move that shortcut into the shell startup folder

- This should autorun the website, which points to that youtube playlist in fullscreen allowing you to use it as a background for displays for parties or just a general display
  - To make the most of this install an adblocker like Ublock plus something to remove Youtube recommended videos like Unhook Youtube to remove next video suggestions and ads.

Worth mentioning: It's possible to just run the file locally as an HTML file and point to it but youtube will not allow Iframes to play certain videos due to their referrer policy, or the owner disabling embedded sharing, I tried with different referrer policies but had no luck.
I think it's because the site being run locally does not HTTPS enabled so it prevents videos from playing so the display will stop on any video with the issue, to get around this I deployed it to my own domain 
