# Bluesky Repost Hider
A simple script that adds a button to toggle reposts on a bluesky user's profile.<br>
Mobile UI and theme compatible.

### Function
Adds a button above the section navbar on all Bluesky profile pages: (it also stays on screen when scrolling down)

![image](https://github.com/user-attachments/assets/ab97c75b-3a94-4b36-bafa-a326f2a61cb2)

When pressed, the button will toggle the state of all posts that are found to be a repost (this is determined by checking if the `data-testid` of each post does not match the profile being viewed). In addition, it starts an interval to check for newly loaded posts, so it responds well to scrolling.

### Known Issues
- the css transition is a little janky, especially on much longer profile feeds
- no configurable options
- the show/hide state does not persist across other tabs / reloads
