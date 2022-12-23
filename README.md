# smartphone-device
A 360px wide screen smartphone layout for previewing and confirming responsive website features

Developed with only CSS
```css
    /* The device with borders */
    .smartphone {
      position: relative;
      width: 360px;
      height: 640px;
      margin: auto;
      border: 16px black solid;
      border-top-width: 50px;
      border-bottom-width: 50px;
      border-radius: 36px;
    }

    /* The horizontal line on the top of the device */
    .smartphone:before {
      content: "";
      display: block;
      width: 60px;
      height: 5px;
      position: absolute;
      top: -30px;
      left: 50%;
      transform: translate(-50%, -50%);
      background: #333;
      border-radius: 10px;
    }

    /* The circle on the bottom of the device */
    .smartphone:after {
      content: "";
      display: block;
      width: 35px;
      height: 35px;
      position: absolute;
      left: 50%;
      bottom: -65px;
      transform: translate(-50%, -50%);
      background: #333;
      border-radius: 50%;
    }

    /* The screen (or content) of the device */
    .smartphone .content {
      width: 360px;
      height: 640px;
      background: white;
    }

```

```html
<!DOCTYPE html>
<html>

<head>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <link rel="stylesheet" href="style.css" />
</head>

<body>
  <div class="smartphone">
    <div class="content">
      <iframe src="http://localhost" style="width: 100%; border: none; height: 100%"></iframe>
    </div>
  </div>
</body>

</html>
```
