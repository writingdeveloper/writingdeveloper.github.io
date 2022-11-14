---
title: How to check if a chrome extension is installed with javascript
date: 2022-11-14 20:40:00 +09:00
categories: [Programming, JavaScript]
tags: [javascript, chrome extension] # TAG names should always be lowercase
---

# How to check if a chrome extension is installed with javascript

I'm currently developing a Chrome Extension program. I suddenly wondered if I could implement a function that guides the installation page by checking the website for the installation of the extension program I made.

## Solution

I found a solution in StackOverflow. There are various ways to check it, but I found this way is the easiest way.

[**Use Connection Method**](https://developer.chrome.com/extensions/extension#global-events)

```javascript
let check = chrome.extension.connect(
  "extension id in chrome developer dashboard",
  some_object_to_send_on_connect
);
```
