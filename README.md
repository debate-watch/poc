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

### installing bower

```` sh
npm install bower
````

### installing packages from bower config (if already populated)

```` sh
bower install
````

### populate bower config upon package installation

```` sh
bower install <package> --save
````

### starting web server

```` sh
python -m SimpleHTTPServer 8888 &
````
