# Top and Lock It

The topAndLockIt function takes a jQuery element and a set of values to interpolate.

As the element approaches the top of the window, it will interpolate the values of the given css attributes towards the values passed in as an argument and away from their original values.

Once the element hits the top of the window, it will be locked into place at the top.

``` html
<!DOCTYPE HTML>
<html>
  <head>
    <meta http-equiv="content-type" content="text/html; charset=utf-8">
    <script src="jquery.js"></script>
    <script src="top-and-lock-it.js"></script>
    <script>
      $(function () {
        topAndLockIt($("#thing"), {
          width:   50,
          height:  50,
          opacity: 1.0
        })
      })
    </script>
    <style>
      body {
        height: 2000px;
      }

      #thing {
        margin-top: 400px;
        background: red;
        width: 100px;
        height: 100px;
        opacity: 0.5;
      }
    </style>
  </head>
  <body>
    <div id="thing"></div>
  </body>
</html>
```
