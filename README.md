# Minutes

Minimalist light weight new tab browser extension for your Firefox browser.
 Based on Traversy Media dynamic landing page tutorial which is inspired by Moment / Momentum extension.

##### Features
- Minimal and light weight
- The backgroud and greeting will change based on the time of the day
- Name and Focus message can be changed


[Traversy Media Youtube Link](https://www.youtube.com/watch?v=fSTQzlprGLI)

[Firefox Extensions Link](https://addons.mozilla.org/en-US/firefox/addon/minutes/)

Screenshot:

![Main Screenshot](/images/screenshot1.png?raw=true)

##### Remove extension name from urlbar

1. Enable `toolkit.legacyUserProfileCustomizations.stylesheets` using `about:config` 
2. Create `userChrome.css` in your profile folder and add the following lines.

```css
#identity-box.extensionPage #identity-icon-label {
	visibility: collapse !important;
	transition: visibility 250ms ease-in-out;
}
	#identity-box.extensionPage:hover #identity-icon-label {
	visibility: visible !important;
	transition: visibility 250ms ease-in-out 500ms;
}
```
##### User Styles Enabled
![FF URL BAR](/images/Screenshot-ff-stylesheet?raw=true)
