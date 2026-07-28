There are two scripts you could use if one or another doesn't work. This just speeds up the video to 10x, nothing else.  


the first one: document.querySelector('video').playbackRate = 10;




the second one: setInterval(() => {
  const video = document.querySelector('video');
  if (video && video.playbackRate !== 10) {
    video.playbackRate = 10;
  }
}, 500);
