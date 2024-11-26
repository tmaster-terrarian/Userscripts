# Bluesky Repost Hider
[github](https://github.com/tmaster-terrarian/Userscripts/tree/main/Bluesky%20Repost%20Hider) | [greasy fork](https://greasyfork.org/en/scripts/518654-bluesky-repost-hider)

A simple script that adds a button to toggle reposts on a bluesky user's profile.<br>
Mobile UI and theme compatible.

![image](https://raw.githubusercontent.com/tmaster-terrarian/Userscripts/main/Bluesky%20Repost%20Hider/preview.png)

When pressed, the button will toggle the state of all posts that are found to be a repost (this is determined by checking if the `data-testid` of each post does not match the profile being viewed). In addition, it starts an interval to check for newly loaded posts, so it responds well to scrolling.

### Known Issues
- the css transition is a pretty janky on much longer profile feeds
- the show/hide state does not persist
- can occasionally fail on first page load, a temporary fix is to simply reload the page and pray
- does not hide self-reposts

### Planned Features
- actually functional scroll persistence
- localStorage usage to keep the state intact when opening new tabs and/or reloading
