# Credits, Notes, and Reference

## Video Sources

 + [C-SPAN](http://www.c-span.org)
 + [Youtube](http://youtube.com)

## Video Downloading

 + [youtube-dl](https://github.com/rg3/youtube-dl)

```` sh
youtube-dl http://www.c-span.org/video/?326473-1/donald-trump-presidential-campaign-announcement \
  --write-info-json \
  --restrict-filenames \
  --output "%(epoch)s-%(extractor_key)s-%(id)s-%(format_id)s-%(title)s.%(ext)s"
````

produces...

```` json
{
  "display_id": "403512",
  "extractor": "CSpan",
  "playlist": null,
  "description": "Business magnate Donald Trump announced his intention to seek the 2016 Republican presidential nomination in remarks at Trump Tower in New York.\u2002He was introduced by his daughter, Ivanka Trump.",
  "format": "0 - unknown",
  "url": "http://d19cp144waw2mw.cloudfront.net/trimmed/program/040/403512/program.403512.MP4-D20.mp4?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cDovL2QxOWNwMTQ0d2F3Mm13LmNsb3VkZnJvbnQubmV0L3RyaW1tZWQvcHJvZ3JhbS8wNDAvNDAzNTEyL3Byb2dyYW0uNDAzNTEyLk1QNC1EMjAubXA0IiwiQ29uZGl0aW9uIjp7IkRhdGVMZXNzVGhhbiI6eyJBV1M6RXBvY2hUaW1lIjoxNDM0NjE4MDg5fSwiSXBBZGRyZXNzIjp7IkFXUzpTb3VyY2VJcCI6IjczLjIxOS4yMjMuNjEifX19XX0_&Key-Pair-Id=APKAIHKVWBEAXX562G7Q&Signature=k5GrkUBMoQ6l~bRcKgSBeEVQH5Uxfg8LkaoSJDEDMD9S-x1-Ku2yI2wzyosa6eCl3lSP3lp24rI8vAfGncPS2MFk7fGNY34AxcGwv07WsLsx3ka4UaooIOa~kj-2j-ivhhQoaZXraqo-um-MHa9Y3rB14c7O5uLt2b1zonjkEhU_",
  "extractor_key": "CSpan",
  "title": "Donald Trump Presidential Campaign Announcement",
  "playlist_index": null,
  "thumbnail": "http://images.c-spanvideo.org/Files/061/20150616110806003_hd.jpg",
  "ext": "mp4",
  "fulltitle": "Donald Trump Presidential Campaign Announcement",
  "webpage_url_basename": "video",
  "webpage_url": "http://www.c-span.org/video/?326473-1/donald-trump-presidential-campaign-announcement",
  "_filename": "Donald Trump Presidential Campaign Announcement-403512.mp4",
  "duration": 3412,
  "format_id": "0",
  "http_headers": {
    "Accept-Charset": "ISO-8859-1,utf-8;q=0.7,*;q=0.7",
    "Accept-Language": "en-us,en;q=0.5",
    "Accept-Encoding": "gzip, deflate",
    "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
    "User-Agent": "Mozilla/5.0 (X11; Linux x86_64; rv:10.0) Gecko/20150101 Firefox/20.0 (Chrome)"
  },
  "id": "403512",
  "subtitles": {
    "en": [
      {"url": "http://data.c-spanvideo.org.s3.amazonaws.com/Programs/403/403512/1434513231.dfxp", "ext": "dfxp"}
    ]
  },
  "thumbnails": [
    {"url": "http://images.c-spanvideo.org/Files/061/20150616110806003_hd.jpg", "id": "0"}
  ]
}
````

## Video Playing
### Local Files (from CSpan or YouTube)
 + https://github.com/jwplayer/jwplayer
   + [api key management](https://account.jwplayer.com/#/account)
   + [quick-start](http://support.jwplayer.com/customer/portal/articles/1413074-javascript-api-quick-start)
   + [api docs](http://support.jwplayer.com/customer/portal/articles/1413089-javascript-api-reference)
   + [logo removal. hmm...](http://support.jwplayer.com/customer/portal/articles/1406865-branding-your-player)
   + [notes and comments](https://gist.github.com/s2t2/45460c06581798ba6e94#file-jwplayer_notes-js)
   + [gitter chat](https://gitter.im/jwplayer/jwplayer)

### Embedded Videos (from YouTube)
 + http://stackoverflow.com/questions/6970013/getting-current-youtube-video-time
 + [youtube iframe api reference](https://developers.google.com/youtube/iframe_api_reference)
 + [jwplayer `onTime()` function equivalency](http://stackoverflow.com/questions/16687995/youtube-api-equivalent-of-ontime)

## Site Branding and Management
 + [podium icon](https://cdn4.iconfinder.com/data/icons/businessmen-set-1/512/30-512.png)
 + [octocons](https://octicons.github.com/usage/)
 + [bower](http://bower.io/docs/creating-packages/#bowerjson)

## Site Controls
 + [svg lines](https://github.com/mbostock/d3/wiki/SVG-Shapes#svg_line)
 + [jquery ui slider api](http://api.jqueryui.com/slider/)
   + [avoiding `Maximum call stack size exceeded` (infinite loop) when re-setting slider value from inside the `change` event](https://forum.jquery.com/topic/setting-a-sliders-value-without-triggering-the-change-event#14737000000537461)
 + [slider pips (tooltips & tick-marks)](https://github.com/simeydotme/jQuery-ui-Slider-Pips)
   + [slider tooltips & tick-marks customization](http://simeydotme.github.io/jQuery-ui-Slider-Pips/#customisation-styling)
 + [circular slider](https://github.com/princejwesley/circular-slider)

## Data Collection and Visualization
 + [d3 line chart](http://bl.ocks.org/mbostock/3883245)
 + [d3 line generation function](https://github.com/mbostock/d3/wiki/SVG-Shapes#path-data-generators)
 + [creating d3 line graphs](http://www.sitepoint.com/creating-simple-line-bar-charts-using-d3-js/)
 + [d3 array map](https://github.com/mbostock/d3/wiki/Arrays#d3_map)
 + [d3 transition](https://github.com/mbostock/d3/wiki/Transitions#d3_transition)
 + [svg paths and d3](https://www.dashingd3js.com/svg-paths-and-d3js)

## Data Capture and Storage
### Rails
 + [jquery-post-to-rails](http://stackoverflow.com/questions/7237720/jquery-post-to-rails)
 + [jquery-ajax-post-function-rails](http://stackoverflow.com/questions/7832069/jquery-ajax-post-function-rails)

### Redshift
 + [aws javascript sdk](https://github.com/aws/aws-sdk-js)
 + [aws javascript sdk- getting started](http://docs.aws.amazon.com/AWSJavaScriptSDK/guide/browser-intro.html)

### Mongo
 + meh
