console.log({
    seek: document.querySelector('#seek'),
    seekHTML: document.querySelector('#seek')?.outerHTML,
    videoCount: document.querySelectorAll('video').length,
    videos: [...document.querySelectorAll('video')].map(v => ({
        duration: v.duration,
        currentTime: v.currentTime,
        paused: v.paused,
        src: v.currentSrc
    }))
});
