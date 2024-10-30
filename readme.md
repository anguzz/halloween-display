- On windows desktop create a new shortcut
- use the following, which will open it up in fullscreen kiosk mode 
"C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" --kiosk "https://h.angs.dev/"
- Now use windows+R to run shell:startup
- Move that shortcut into the shell startup folder

- This should autorun the website, which has points to that youtube playlist in fullscreen allowing you to use it as a background for displays for parties or just a general display
  - To make the most of this install an adblocker like Ublock plus something to remove Youtube recommended videos like Unhook Youtube to remove next video suggestions and ads.

Worth mentioning: It's possible to just run the file locally as an HTML file and point to it but youtube will not allow Iframes to play videos, I tried with different referrer policies but had no luck.
I think it's because the site being run locally does not HTTPS enabled so it prevents videos from playing so the display will break 
