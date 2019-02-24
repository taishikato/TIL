# Create a 360 Panorama viewer

I use [Panolens](https://pchen66.github.io/Panolens/) for this.  
It's so easy to make it :thumbsup:

<img width="350" alt="360viewer" src="https://user-images.githubusercontent.com/980588/53295384-85c5bd00-383d-11e9-839d-4b3ec3a7e8f8.png">

```html
<!DOCTYPE HTML>
<html>
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Auto load</title>
    <link rel="stylesheet" href="https://cdn.pannellum.org/2.4/pannellum.css"/>
    <script type="text/javascript" src="https://cdn.pannellum.org/2.4/pannellum.js"></script>
    <style>
    #panorama {
        width: 600px;
        height: 400px;
    }
    </style>
</head>
<body>

<div id="panorama"></div>
<script>
pannellum.viewer('panorama', {
    "type": "equirectangular",
    "panorama": "1.JPG",
    "autoLoad": true
});
</script>

</body>
</html>
```
