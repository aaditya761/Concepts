# Concepts


# How a browser works

### Parts of a web browser:

* ##### User Interface
this includes the address bar, back/forward button, bookmarking menu, etc. Every part of the browser display except the window where you see the requested page
* ##### The browser engine: 
marshals actions between the UI and the rendering engine.
* ##### The rendering engine : 
responsible for displaying requested content. For example if the requested content is HTML, the rendering engine parses HTML and CSS, and displays the parsed content on the screen. By default the rendering engine can display HTML and XML documents and images. It can display other types of data via plug-ins or extension; for example, displaying PDF documents using a PDF viewer plug-in. Different browsers use different rendering engines: Internet Explorer uses Trident, Firefox uses Gecko, Safari uses WebKit. Chrome and Opera (from version 15) use Blink, a fork of WebKit.
* ##### Networking: 
for network calls such as HTTP requests, using different implementations for different platform behind a platform-independent interface.
* ##### UI backend: 
used for drawing basic widgets like combo boxes and windows. This backend exposes a generic interface that is not platform specific. Underneath it uses operating system user interface methods.
* ##### JavaScript interpreter. 
Used to parse and execute JavaScript code.
* ##### Data storage. 
This is a persistence layer. The browser may need to save all sorts of data locally, such as cookies. Browsers also support storage mechanisms such as localStorage, IndexedDB, WebSQL and FileSystem.

It is important to note that browsers such as Chrome run multiple instances of the rendering engine: one for each tab. Each tab runs in a separate process.

![alt text](https://www.html5rocks.com/en/tutorials/internals/howbrowserswork/layers.png)

