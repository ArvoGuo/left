Just bind once, run on mobile and pc;

Mix mobile events and pc events, extreme simple way to addEventListener;

You just need to bind "touchstart", it take effect as "mousestart" of "touchstart" according to [IsMobile];

Usage:

```
var a = document.getElementsByTagName('body')

// or var a document.getElementsByTagName('body')[0]

a.on('touchstart', function() {
    //do something
});

```

Note:

```
for the moment it only support:

-------------------------------
|  PC         |   Mobile      |
-------------------------------
|  click      |   click       |
-------------------------------
|  mousestart |   touchstart  |
-------------------------------
|  mousemove  |   touchmove   |
-------------------------------
|  mouseend   |   touchend    |
-------------------------------


```