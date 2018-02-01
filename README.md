<!DOCTYPE html>
<html>
  <head>
    <title>Integrate</title>
    <meta name="viewport" content="width=device-width,
                                   initial-scale=1.0,
                                   maximum-scale=1.0,
                                   user-scalable=no,
                                   minimal-ui">
    <link rel="stylesheet" href="//cdn.kik.com/app/3.0.0/app.min.css">
    <style>
      /* put your styles here */
    </style>
  </head>
  <body>
    <!-- put your pages here -->
    <script src="//zeptojs.com/zepto.min.js"></script>
    <script src="//cdn.kik.com/app/3.0.0/app.min.js"></script>
    <script>
      /* put your javascript here */
    </script>
  </body>
</html>

<div class="app-page">
  <div class="app-topbar"></div>
  <div class="app-content"></div>
</div>

<div class="app-topbar">
  <div class="app-button left" data-back>Profile</div>
  <div class="app-title">Integrate</div>
  <div class="app-button right">Messages</div>
</div>

<div class="app-page" data-page="home">
  <div class="app-topbar"></div>
  <div class="app-content"></div>
</div>

 
/* in your javascript */
App.controller('home', function (page) {
    .find('.app-button')
    .on('click', function () {
      console.log('button was clicked!');
    });
});

App.load('home');

