# debate watch

## process notes

### setting up development environment

```` sh
brew install youtube-dl
````

### downloading videos from the web

```` sh
youtube-dl http://www.c-span.org/video/?326033-1/iowa-gop-lincoln-dinner
````

> ensure compliance with video provider terms and conditions

### starting web server

```` sh
python -m SimpleHTTPServer 8888 &
````
