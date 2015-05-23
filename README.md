# debate watch

## development environment notes

### downloading videos from the web

```` sh
brew install youtube-dl

(or)

sudo curl https://yt-dl.org/latest/youtube-dl -o /usr/local/bin/youtube-dl
sudo chmod a+x /usr/local/bin/youtube-dl
````

```` sh
youtube-dl http://www.c-span.org/video/?326033-1/iowa-gop-lincoln-dinner
````

> ensure compliance with video provider terms and conditions

### using octocons icons

```` sh
npm install bower
bower install
````

### starting web server

```` sh
python -m SimpleHTTPServer 8888 &
````
