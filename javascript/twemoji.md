I am curious in [Twemoji](https://twemoji.twitter.com/) and just tried it!  
It's so easy!!

### Code

```html
<html>
  <head>
    <style>
      img.emoji {
        height: 2em;
        width: 2em;
        margin: 0 .05em 0 .1em;
        vertical-align: -0.1em;
      }
    </style>
  </head>
  <body>
    😀👽
    <script src="http://twemoji.maxcdn.com/2/twemoji.min.js?12.0.0"></script>
    <script>
      twemoji.parse(document.body);
    </script>
  </body>
</html>
```

### Output
<img width="232" alt="twemoji-output" src="https://user-images.githubusercontent.com/980588/56707310-43dcc880-6753-11e9-8c0b-5b9bb78bec5c.png">
