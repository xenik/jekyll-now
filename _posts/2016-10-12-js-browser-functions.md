---
layout: post
title: pretty information for JS in browser 
---

pretty good

https://www.youtube.com/watch?v=dk75fqFXwCE&index=7&list=PLLnDCesoFbdGmCPt4mhX2XnGoPhgcJYQo

window.performance.timing
window.requestAnimationFrame()


That is the custom event:

var myElement = document.getElementsByTagName('body')[0];
myElement.addEventListener("userLogin", function(e) {
	console.info("Event is: ", e);
	console.info("Custom data is: ", e.detail);
});

// First create the event
var myEvent = new CustomEvent("userLogin", { detail: { username: "davidwalsh"	} });

myElement.dispatchEvent(myEvent);
