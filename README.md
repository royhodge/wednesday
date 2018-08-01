<center>

A Graphical Wallet For MultiChain Blockchains
---------------------------------------------
<br>
Built with :heart: by volunteers under the guidance of UniBit Labs. <br>
<br>

![Current Status](https://img.shields.io/badge/Project%20Status-Work%20In%20Progress-red.svg?longCache=true&style=social "Current Status")

<br>
You have been warned.<br>
<br>
<br>
What is Electron? <br>
<br>

>  Electron is a framework for creating native applications with web technologies like JavaScript, HTML, and CSS. 

<br>
What does this mean to <b>you</b>?<br>
<br>
If you can build a website, then you can now build a desktop app by using Electron.<br>
It takes care of the hard parts so you can focus on the core of your application.<br>
<br>
<br>
We have also chosen to implement <b>Bootstrap</b> because:
<br>
<br>

> Bootstrap is the most popular HTML, CSS, and JS framework in the world for building responsive, mobile-first projects on the web

<br>
* It also happens to require <b>jQuery</b> which also comes in handy for web development.
<br>
<br>

> We are going after the [Look & Feel](https://exodus.io) of the wallet that made crypto beautiful.<br>

>> Please take note of any features to be included during UI/UX sprints please.

<br>

App Preview
-----------

![demo](https://image.ibb.co/hZTx3d/demo_picture.png)

<hr>

Quick Code Tour
---------------

So, This is what I have thrown together for us to use as a starting point.<br>

 - The code entry point is in **package.json** under the key "main". The value is "main.js"<br>
 
 - **main.js** creates a BrowserWindow and loads **index.html**. <br>
 <br>
 
 It also has event handlers that enable keyboard shortcuts for Developer Tools on various platforms. <br>
 <br>
 
 - **index.html** loads Bootstrap's CSS in the &lt;head&gt; tag and **renderer.js** after the closing &lt;body&gt; tag. <br>
 <br>
 
 On the web Bootstrap's JavaScript would also load in this location,<br>
 but the Electron way is to load it in **renderer.js** with a require(). <br>
 <br>
 
 Note that these src and href attributes use normal relative paths. An HTTP server is not necessary.<br>
 <br>
 
 - **renderer.js** loads jQuery, Bootstrap and it's dependency; Tether. <br>
 <br>
 Each is assigned to the window object because this is the web application custom. <br>
 It's not the Node.js or Electron custom because window is a global. <br>
 For now we must do it this way or it won't work.<br>
<br>

 - **config.json** holds the blockchain parameters used for connecting.
 <br>
 <br>
 <br>
 
 --------------------------------------------------------------------------------------------------------
 
 <br>
 <strong>
 DEPENDENCY INFORMATION BELOW:
 </strong>
 <br>
 <br>
 <br>
 
 - **Bootstrap v4.0.0-beta.3**
 > **Bootstrap** is the most popular HTML, CSS, and JavaScript framework for developing responsive, mobile first projects.
 <br>
 
 - **jQuery v3.2.1**
 > **jQuery** is a JavaScript Library.
 <br>
 
 - **tether v1.4.0**
> **tether** is a positioning engine to make overlays, tooltips and dropdowns better.
 <br>
 
 - **Electron v2.0.3**
 > **Electron** is "One Of The Best" frameworks for creating native applications. (In our opinion, at this point in time.)
 <br>
 
 - **multichain-api v1.0.0-alpha.8**
 > **multichain-api** is an unofficial MultiChain client written for Node.js
 <br>
 
 - **multichain-node v2.1.6-version1.0.2**
 > **multichain-node** is a native Javascript client built for Multichain.
 <br>
 
 - **Bluebird v3.5.1**
 > **bluebird** is a fully featured promise library.
 <br>
 
 - **popper.js v1.12.9**
 > **popper.js** is "a kickass library used to manage poppers in web applications".
 <br>
 
 - **intro.js v2.9.3**
 > **intro.js** is a step-by-step guide for your project. 
 <br>
 
 - **open-file-text-editor v0.0.1**
 > **open-file-text-editor** will open files in text editor.
 <br>
 
 <br>
 - **ALL OTHER APP DEPENDENCIES NEED LISTED!!** and what they are doing or providing for our app's functionality..
 
</center>
