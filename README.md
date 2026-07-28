There are two scripts you could use if one or another doesn't work. This just speeds up the video to 10x, nothing else.  


### 1. One-Time Speed Boost

**console-boost.js**
```javascript
document.querySelector('video').playbackRate = 10;
```

---

### 2. Continuous Speed Lock

**console-loop.js**
```javascript
setInterval(() => {
  const video = document.querySelector('video');
  if (video && video.playbackRate !== 10) {
    video.playbackRate = 10;
  }
}, 500);
```




How to use: press F12 on your keyboard and paste this in the console. 
