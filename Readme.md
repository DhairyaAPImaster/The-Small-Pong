# The small Pong.


This is (as the name suggests) is a version of a ping pong game in which there is one paddle and there is 1 ball. Now what happens is that the ball bounces around the screen whith the aim of the player being to hit the ball and prevent it from touching the bottom of the screen. If the ball touches the bottom of the screen then ITS GAME OVER!!!

**The interesting thing about this game is that it is way under just 3kb, it is just 1.897kb, and also u do not need to visit a website to play this as it is fully playable through just a single line data url!!!**


## How can u play it? 

Just copy the following and paste it in your browser and u wil be able to play this!!!--> 

```
data:text/html,<!DOCTYPE html><html lang="en"><head><meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1"><title>Ping Pong</title><style>*{box-sizing:border-box}html,body{margin:0;width:100%25;height:100%25;overflow:hidden;background:%23111}canvas{display:block;width:100%25;height:100%25;cursor:none}</style></head><body><canvas id="game"></canvas><script>const t=document.getElementById("game"),e=t.getContext("2d");let n,i,x=0,f=0;const y={x:0,y:0,r:9,vx:4,vy:4},l={x:0,y:0,w:120,h:14};function o(){n=t.width=window.innerWidth,i=t.height=window.innerHeight,l.y=i-50}function r(){y.x=n/2,y.y=i/3,y.vx=4,y.vy=4,l.x=n/2-l.w/2,l.y=i-50,f=0}function c(t){l.x=t-l.w/2,l.x<0&&(l.x=0),l.x+l.w>n&&(l.x=n-l.w)}function s(){0!==x?2===x&&(r(),x=1):x=1}window.addEventListener("resize",o),t.addEventListener("mousemove",function(t){c(t.clientX)}),t.addEventListener("touchmove",function(t){c(t.touches[0].clientX),t.preventDefault()},{passive:!1}),t.addEventListener("click",function(){s()}),t.addEventListener("touchstart",function(t){s(),t.preventDefault()},{passive:!1}),o(),r(),function t(){!function(){if(1===x){if(y.x+=y.vx,y.y+=y.vy,y.x-y.r<=0&&(y.x=y.r,y.vx*=-1),y.x+y.r>=n&&(y.x=n-y.r,y.vx*=-1),y.y-y.r<=0&&(y.y=y.r,y.vy*=-1),y.y+y.r>=l.y&&y.y-y.r<=l.y+l.h&&y.x>=l.x&&y.x<=l.x+l.w&&y.vy>0){y.y=l.y-y.r,y.vy*=-1;const t=(y.x-(l.x+l.w/2))/(l.w/2);y.vx=7*t,f++}y.y-y.r>i&&(x=2)}}(),e.clearRect(0,0,n,i),e.beginPath(),e.arc(y.x,y.y,y.r,0,2*Math.PI),e.fillStyle="%23fff",e.fill(),e.fillStyle="%23fff",e.fillRect(l.x,l.y,l.w,l.h),e.font="24px system-ui",e.textAlign="center",e.fillStyle="%23fff",e.fillText(f,n/2,40),0===x&&(e.font="20px system-ui",e.fillText("CLICK TO START",n/2,i/2)),2===x&&(e.font="32px system-ui",e.fillText("GAME OVER",n/2,i/2),e.font="18px system-ui",e.fillText("CLICK TO RESTART",n/2,i/2+35)),requestAnimationFrame(t)}();</script></body></html>
```


## How to play? 


This is pretty straightforward and simple->

There is a ball and a paddle and the game begins when u click on it. Then the ball shall go down towards it and the paddle follows your mouse pointer so u need to get the paddle under the ball to bounce it away from the bottom of the screen since if it touches it then its GAME OVER and u lose "SKIBIDI AURA INFINITE"



## PIC'S (of the game) -->


<img width="1918" height="870" alt="image" src="https://github.com/user-attachments/assets/2edb89af-0c07-430e-b49a-4e813daacdad" />


<img width="1918" height="874" alt="image" src="https://github.com/user-attachments/assets/0bea0316-4cc8-48e2-b46e-9551b92217dd" />


<img width="958" height="436" alt="image" src="https://github.com/user-attachments/assets/992f5a75-9283-44e8-8017-47139b90cb38" />



## HAVE FUN PLAYING!!!!






***Made for shrink.hackclub.com (one of the best ysws out there)***



Credits-->

- Thanks to shrink.hackclub.com to help me learn how to make webapps in a data url (before this i honestly didnt know this could be done... so i present to u my first data url web app!!!)
