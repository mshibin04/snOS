# snOS - Personal Web Operating System

This project is a desktop environment running in the browser made with plain HTML, CSS, and JS. It uses glassmorphism, floating interactive windows, depth layering, and built-in web desktop applications.
---

## 🚀 Features

- About snOS Window
Includes information cards about the OS and its creator's avatar.

- Notes App Pro
Built-in notepad utilizing `localStorage()` so that notes are saved even after the browser is reloaded.

- Live Weather Forecast App
Live weather forecast using the `Open-Meteo` API so that users can type in any city and get a live report of the weather, temperature, wind, and other conditions.

- Integrated Web Browser (Custom Feature)
A custom frame window that opens any website directly on the desktop environment.
- Window Management
Includes draggable windows, `zIndex` layering so that only one window is in front, and close buttons.
---
## 🛠️ Built With
- HTML5 & CSS3
- JavaScript
- Open-Meteo API
---
## 📝 Devlogs
### Devlog 1: Desktop Shell & Window Dragging
Created the desktop environment, including a glassmorphism top bar, clock, icons, and windows using HTML and CSS.
Made the desktop icons draggable with a little help from a `makeDraggable()` JavaScript function that follows the cursor's X and Y positions.
### Devlog 2: Persistent Notes app & Layering
Created a working desktop Notes application and icon with a draggable window using the same `makeDraggable()` function from before.
Added event listeners to the Notes app that utilizes `localStorage()` to save whatever text is being written every time the page is refreshed or closed.
Made the Notes window utilize a `bringToFront()` function so that it uses a higher `zIndex` than other windows so that it can be layered on top of other windows.
### Devlog 3: Live Weather Forecast App
Built the Weather Forecast app with an input field and keyboard listener for the "Enter" key.
Used asynchronous `fetch()` requests to the `Open-Meteo` API to get temperature, wind, and weather data and displayed it on the Weather Forecast Window.
### Devlog 4: Custom Feature - Web Browser
Created a Web Browser application with an address bar and frame display utilizing `iframe`.
Might have gone a bit too in-depth with the address bar by making it check if an inputted address begins with `https://`. If it does not, it will add it to the beginning of the address bar text, so it can be displayed as a working website in the frame.
