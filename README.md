<p align="center"> <b>Fork of</b><br/><img src="/docs/logo.svg?sanitize=true&raw=true" width="400"></p>

<hr/>
<p align="center">

<img src="https://img.shields.io/github/last-commit/lizardking/AsyncElegantOTA.svg?style=for-the-badge" />
&nbsp;
<img src="https://img.shields.io/travis/com/lizardking/AsyncElegantOTA/master?style=for-the-badge" />
&nbsp;
<img src="https://img.shields.io/github/license/lizardking/AsyncElegantOTA.svg?style=for-the-badge" />
</p>
<hr/>


<p align="center">Perform OTAs for ESP8266 & ESP32 Asynchronously</p>
<p align="center">
This is a fork of the AsyncElegantOTA library with added support for digest authentication.<br/> <br/>
AsyncElegantOTA provides a beautiful interface to upload Over the Air `.bin` updates to your ESP Modules with precise status and progress displayed over UI. This Library shows the current upload progress of your OTA and once finished, it will display the status of your OTA. This Version of Library uses AsyncWebServer. Thanks to @me-no-dev for a wonderful webserver library.
</p>

<br>
<br>

<h2 align="center">Preview</h2>
<p align="center"><img src="/docs/elegantOtaDemo.gif?raw=true"></p>

<br>
<br>

<h2>How to Install</h2>

###### Directly Through Arduino IDE ( Currently Submitted for Approval. Use Mannual Install till it gets Approved.)
Go to Sketch > Include Library > Library Manager > Search for "AsyncElegantOTA" > Install

###### Manual Install

For Windows: Download the [Repository](https://github.com/ayushsharma82/AsyncElegantOTA/archive/master.zip) and extract the .zip in Documents>Arduino>Libraries>{Place "ElegantOTA" folder Here}

For Linux: Download the [Repository](https://github.com/ayushsharma82/AsyncElegantOTA/archive/master.zip) and extract the .zip in Sketchbook>Libraries>{Place "ElegantOTA" folder Here}

###### Manually through IDE

Download the [Repository](https://github.com/ayushsharma82/AsyncElegantOTA/archive/master.zip), Go to Sketch>Include Library>Add .zip Library> Select the Downloaded .zip File.

<br>

<h2>Documentation</h2>
<p>AsyncElegantOTA is a dead simple library which does your work in just 1 Line. Honestly, It's just a wrapper library which injects it's own elegant webpage instead of the ugly upload page which comes by default in Arduino Library.</p>

 Include AsyncElegantOTA Library `#include <AsyncElegantOTA.h>` at top of your Arduino Code.
 
 Paste this - `AsyncElegantOTA.begin(&server, authenticationRealm, authenticationHash);`  line above your `server.begin();`
 The values for authenticationRealm and authenticationHash must be defined in your code resp. loaded from config data.
 
 Past this -   `AsyncElegantOTA.loop();` line into the loop of your code.
 
 That's all!
 
 Now copy the IPAddress displayed over your Serial Monitor and go to `http://<IPAddress>/update` in browser. ( where `<IPAddress>` is the IP of your ESP Module)
 
<br>
<h2>Examples</h2>
 


<br>
<br>

<h2>Contributions</h2>
<p>Every Contribution to this repository is highly appriciated! Don't fear to create pull requests which enhance or fix the library as ultimatly you are going to help everybody.</p>
<p>
If you want to donate to the author then <b>you can buy me a coffee</b>, It really helps me keep these libraries updated:


<h2>License</h2>
ESP-DASH is licensed under MIT.
<br/>
<br/>
<img src="https://img.shields.io/github/license/lizardking/AsyncElegantOTA.svg?style=for-the-badge" />
</div>
