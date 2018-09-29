# *YasinEhsan.github.io*

**Version 2.0.0**

[Portfolio site](https://yasinehsan.com/) hosted using Git Pages.

## To Do
- [ ] Connect with Google Analytics
- [ ] Add Thumbnail
- [ ] Add Bookmark Icon
- [ ] Projects Text
- [ ] Articles Text
- [ ] Skills Text
- [ ] \(Maybe) button for freelance

## Video Walkthrough
<img src='http://i.imgur.com/link/to/your/gif/file.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />

GIF created with [LiceCap](http://www.cockos.com/licecap/).

## Useful Links
- [Set up git pages with custom domain](https://medium.com/@kimcodes/setting-up-a-web-page-with-github-pages-f77d45573ab2)
- [SSL with custom domain](https://www.youtube.com/watch?v=UK5-nO4qK9g) *Using CloudFlare or LetEncrypt for SSL not necessary*
- [Set up Google Analytics](https://www.youtube.com/watch?v=mXcQ7rVn3ro)


## Debug Issues
- Trying to access non-SSL certified links from a secure connection will not work. Instead change the URL to without the protocol OR change http links to https.

   Change `http://resources.infolinks.com/js/infolinks_main.js` to `//resources.infolinks.com/js/infolinks_main.js` or `httpS://resources.infolinks.com/js/infolinks_main.js`

- Found warning when I ran Chrome Inspector. Apparently Google Chrome updated Smoothscroll.js. Quick Fix:
   Replace
   ```javascript
    var ischrome = /chrome/.test(navigator.userAgent.toLowerCase());
    if (ischrome) {
        ssc_addEvent("mousedown", ssc_mousedown);
        ssc_addEvent("mousewheel", ssc_wheel);
        ssc_addEvent("load", ssc_init)
    }
   ```
   with
   ```Javascript
   var ischrome = /chrome/.test(navigator.userAgent.toLowerCase());
   if (false) {                          REPLACEMENT
   	ssc_addEvent("mousedown", ssc_mousedown);
   	ssc_addEvent("mousewheel", ssc_wheel);
   	ssc_addEvent("load", ssc_init);
    }
    ```
    **Note:** isChrome is just a variable.













1. Trying to access non-SSL certified links from a secure connection will not work. Instead change the URL to without the protocol OR change http links to https.

   Change `http://resources.infolinks.com/js/infolinks_main.js` to `//resources.infolinks.com/js/infolinks_main.js` or `httpS://resources.infolinks.com/js/infolinks_main.js`

2. Found warning when I ran Chrome Inspector. Apparently Google Chrome updated Smoothscroll.js. Quick Fix:

   Replace
  ```javascript
   var ischrome = /chrome/.test(navigator.userAgent.toLowerCase());
   if (ischrome) {
       ssc_addEvent("mousedown", ssc_mousedown);
       ssc_addEvent("mousewheel", ssc_wheel);
       ssc_addEvent("load", ssc_init)
   }
  ```
  with
  ```Javascript
  var ischrome = /chrome/.test(navigator.userAgent.toLowerCase());
  if (false) {                          REPLACEMENT
  	ssc_addEvent("mousedown", ssc_mousedown);
  	ssc_addEvent("mousewheel", ssc_wheel);
  	ssc_addEvent("load", ssc_init);
   }
   ```
   **Note:** isChrome is just a variable.


- > Trying to access non-SSL certified links from a secure connection will not work. Instead change the URL to without the protocol OR change http links to https.
 >Change `http://resources.infolinks.com/js/infolinks_main.js` to `//resources.infolinks.com/js/infolinks_main.js` or `httpS://resources.infolinks.com/js/infolinks_main.js`	 >>Change `http://resources.infolinks.com/js/infolinks_main.js` to `//resources.infolinks.com/js/infolinks_main.js` or `httpS://resources.infolinks.com/js/infolinks_main.js`
 - Found warning when I ran Chrome Inspector. Apparently Google Chrome updated Smoothscroll.js. Quick Fix:	- >Found warning when I ran Chrome Inspector. Apparently Google Chrome updated Smoothscroll.js. Quick Fix:
> *Replace*	>> *Replace*
 ```javascript	 ```javascript
 var ischrome = /chrome/.test(navigator.userAgent.toLowerCase());	 var ischrome = /chrome/.test(navigator.userAgent.toLowerCase());
 if (ischrome) {	 if (ischrome) {
@@ -25,7 +25,8 @@
```	```
*with*	*with*
```Javascript	```Javascript
If (false) {                          REPLACEMENT	var ischrome = /chrome/.test(navigator.userAgent.toLowerCase());
if (false) {                          REPLACEMENT
	ssc_addEvent("mousedown", ssc_mousedown);		ssc_addEvent("mousedown", ssc_mousedown);
	ssc_addEvent("mousewheel", ssc_wheel);		ssc_addEvent("mousewheel", ssc_wheel);
	ssc_addEvent("load", ssc_init);		ssc_addEvent("load", ssc_init);

## License
© 2018 Yasin Ehsan

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
