Copy As Markdown
================

This is a Chrome Extension used to copy the element in current page as markdown format.

## Usage

You can select any element with html format in the current page and then click the extension icon, the relative text with markdown format will be written into the clipboard. When you select nothing in the page, the page's link will be written to the cliboard, the content is like this: `[window.title](location.href)`.

Also, you can custom the shortcut for the extension in Chrome's tab `chrome://extensions/`, suggested is **Ctrl+Shift+C**.

## Get it From WebStore

<https://chrome.google.com/webstore/detail/copy-as-markdown/dgoenpnkphkichnohepecnmpmihnabdg>

##Source

- https://github.com/JohnnyFee/CopyAsMarkdown

## Issue

- [x] Convert html to markdown.
- [x] Write the resutl(markdown) to clipboard.
- [x] When there is no selection range, copy title and location url.
- [x] Copy the `[title](url)` of the active page to clipboard.
- [ ] add option page for inline link or not.
- [x] Modify extension icon.
- [x] Set shortcut for the browser action.
- [x] Parse the relative url to full.
- [x] i18n. 
- [x] Beatify the href when no selection, such as remove the extra param `utm_*` in the link <http://www.michenux.net/android-around-me-tutorial-974.html?utm_source=Android+Weekly&utm_campaign=292d0789d2-Android_Weekly_88&utm_medium=email&utm_term=0_4eb677ad19-292d0789d2-337832837>. After that, the link will be <http://www.michenux.net/android-around-me-tutorial-974.html>.
- [ ] Modify the running time of content script to idle.
- [x] When copy more relative links, make url all links will be ok!
- [x] Make sure the relative link of images is right!
- [x] Add an option to the option page to filter `|` or not. Simplly reremove the content after `|`.

## Reference

- [kates / html2markdown](https://github.com/kates/html2markdown) Javascript implementation for converting HTML to Markdown text. Browser and Node.js support.
- [evilstreak / markdown-js](https://github.com/evilstreak/markdown-js) 提供Markdown转化为HTML的方法。
- [adam-p / markdown-here](https://github.com/adam-p/markdown-here) Google Chrome, Firefox, and Thunderbird extension that lets you write email in Markdown and render it before sending. 
- [domchristie / to-markdown](https://github.com/domchristie/to-markdown) An HTML to Markdown converter written in javascript 
<http://domchristie.github.com/to-markdown>.
- [rick-li / clipboardExt](https://github.com/rick-li/clipboardExt) Chrome extension to copy current title&url.
