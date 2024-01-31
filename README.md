# Bookmarklets

## Running Bookmarklets

### Normal way
Make a bookmark and replace the URL with the JS code

### The Better way
Start by going to [this link](https://chromewebstore.google.com/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm?pli=1) to get uBlock Origin

![uBlock Origin](https://github.com/Mr-milky-way/Bookmarklets/assets/131718510/e4e08462-71d4-46cd-aff1-9bfe56d7db32)

Next go to [Extensions](chrome://extensions/?id=cjpalhdlnbpafiamejdnhcphjbkeiagm) and find the button that says extension options

![Extension Options](https://github.com/Mr-milky-way/Bookmarklets/assets/131718510/d4d56bda-988e-4cc3-bbb9-f37a6c77899c)

Then scroll down and hit the box that says **I am an advanced user** and then a gear icon will show up, click that.

![I am an advanced user](https://github.com/Mr-milky-way/Bookmarklets/assets/131718510/d71535c6-223c-4732-881d-980f91dd3f7c)

After that find userResourcesLocation and put this code in there: 
```
https://raw.githubusercontent.com/Mr-milky-way/Bookmarklets/main/Ublock/ublockExec.js
```

> [!WARNING]
> **YOU NEED TO HIT APPLY CHANGES.**

![userResourcesLocation](https://github.com/Mr-milky-way/Bookmarklets/assets/131718510/2e442c12-ea12-4730-b130-7599dfdb559e)

Last go back to settings, go to **My Filters**, and put in the code: 
```js
*##+js(execute_script.js)
```
> [!WARNING]
> **YOU NEED TO HIT APPLY CHANGES.**

![My Filters](https://github.com/Mr-milky-way/Bookmarklets/assets/131718510/3f0e2fab-7e67-43b6-9439-dd2b75182f08)

Now all you have to do is hit (ctrl) + (`) and put in your code like this
```js
javascript:(function() {  var scriptElement = document.createElement('script');  var sourceUrl = 'https://raw.githubusercontent.com/Mr-milky-way/better-ego/main/Meun.js';  fetch(sourceUrl)    .then(response => response.text())    .then(sourceCode => {      scriptElement.text = sourceCode;      document.body.appendChild(scriptElement);    })    .catch(error => console.error('Error fetching script:', error));})();
```

## What they do
### [YTSpeed](ytspeed.js)
Speed up the video even more. Also has a slider to dim the video because why not?

Note: At x10 speed, the video usually plays faster than it can load.

This bookmarklet works for videos on other websites too.

### [Tab Title](TabTitle.js)
Lets you retitle tabs and change the favicon.

### [Performance Heatmap](performance_heatmap.js)
Go [here](https://github.com/zeman/perfmap) to see all the info.

### [Rainbow Screen](Rainbow_Screen.js)
Makes the screen rainbow and plays farting noises.
> Not the best idea to use at max volume
### [YTThumb](YTThumb.js)
Get the maximum resolution thumbnail of the current video.
