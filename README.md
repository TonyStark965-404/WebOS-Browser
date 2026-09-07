# WebOS Browser

A lightweight browser built specifically for WebOS projects, bringing web browsing directly into your WebOS environment. Designed to be simple, functional, and easy to integrate into browser-based operating systems.

## How does it look?

### Light Mode:
<img width="1122" height="671" alt="image" src="https://github.com/user-attachments/assets/c72d48c3-ec46-4137-b151-aeb33f77c2e3" />


### Dark Mode:
<img width="1124" height="689" alt="image" src="https://github.com/user-attachments/assets/e30e1096-0845-4e0e-9ad8-b1c9bc82110d" />


[![Click here to launch](https://img.shields.io/badge/Run-Browser-brightgreen?style=for-the-badge)](https://tonystark965-404.github.io/WebOS-Browser/)

## What can it do?

* Browse supported websites directly inside the WebOS environment.
* Navigate using Back, Forward, Home, and Refresh controls.
* Search the web or enter a URL directly through the address bar.
* Has some commonly used/helpful websites as bookmarks.
* View and revisit browsing history.
* Open a new tab.
* Share the current page by copying its URL to the clipboard.
* Light and Dark modes.
* Loading indicator with a stop-style loading state.
* Responsive layout designed for WebOS environments.

## What features does it have?

* A clean and basic interface.
* Custom browser toolbar with navigation controls.
* Address bar with URL detection and web search.
* Bookmark bar for quick access to frequently used websites.
* Built-in browsing history.
* Browser menu with New Tab and History options.
* Clipboard-based link sharing with a confirmation toast.
* Light and Dark themes that can sync with the WebOS theme.
* Designed to work as a browser integration for WebOS projects.

## How can I run it locally and modify it?

Easy, just do this:

```
git clone https://github.com/TonyStark965-404/WebOS-Browser.git
cd WebOS-Browser
```

Open `index.html` in your browser to use it, or open the project in VS Code or a similar editor to modify it.

And if you want to run it in your WebOS,
- Put the cloned folder inside your WebOS directory
- Use `<iframe>` inside the WebOS to refer to the index.html inside the cloned folder.
- Change the background color of document from black to transparent if you want to keep the background from your OS.

>[! NOTE]: You would have to modify the code for both your WebOS and this browser to make it work alongside the theme system (right now the browser refers to the theme of Fluetro OS).

## How does it work?

WebOS Browser is built using HTML, CSS, and JavaScript.

The browser uses an `<iframe>` to display webpages while JavaScript handles navigation, bookmarks, history, theme switching, loading states, and clipboard-based sharing. Browsing history is maintained locally within the browser session.

## Are there any limitations?

Yes, WebOS Browser has some limitations compared to full desktop browsers:

- It uses an `<iframe>` to display webpages, so some websites may refuse to load because of security policies.
- Cross-origin webpages cannot be directly inspected or controlled because of the browser's Same-Origin Policy.
- The browser cannot automatically detect navigation performed inside a cross-origin webpage, so its address bar may not always reflect navigation that happens entirely within an embedded website.
- Browser history is maintained by WebOS Browser itself and is separate from the history of the host browser.
- Some websites may not work correctly because they expect to run as a top-level webpage rather than inside an iframe.
- Features such as browser extensions, downloads, developer tools, private browsing, and advanced browser settings are not included.
- The Dark Mode setting controls the WebOS Browser interface and does not force external websites to use their own dark themes.
- Clipboard sharing requires the browser environment to provide clipboard access.
These limitations are intentional, as WebOS Browser is designed to provide a lightweight browsing experience for WebOS projects rather than act as a complete replacement for a traditional web browser.
