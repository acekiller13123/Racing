 Pixel Racing

Pixel Racing is a lightweight, browser-based retro racing demo built using plain HTML, CSS, and JavaScript. It runs entirely in the browser without any build tools and uses classic pixel-art sprite sheets, simple input handling, and old-school arcade aesthetics.

 Quick Start
Option 1: Open directly

Open the game by launching the HTML file:

pixelracing/index.html
Option 2: Run via a local server (recommended)

Using a local server ensures audio and media load correctly.

Python

python -m http.server

Node.js

npx http-server .

Then open:

http://localhost:8000/pixelracing/index.html
 Controls & Input

Keyboard and game inputs are handled via JavaScript.

Mobile and touch support is included.

Input-related files:

pixelracing/common.js – Core keyboard and input logic

pixelracing/touch.js – Touch and mobile input helpers

 Assets & Sprites
Sprites

Sprite definitions (positions, sizes, offsets) are stored in the SPRITES object.

File:

pixelracing/images/sprites.js
Images

Sprite sheets:

pixelracing/images/sprites/

Background images and logic:

pixelracing/images/background.js
Audio

Music and sound effects are located in:

pixelracing/music/
 Project Structure
pixelracing/
├── index.html
├── common.css
├── common.js
├── touch.js
├── images/
│   ├── background.js
│   ├── sprites.js
│   └── sprites/
├── music/

Additional root files:

.gitattributes
README.md
 Editing & Adding Sprites

To add or modify sprites:

Update the sprite sheet image inside:

pixelracing/images/sprites/

Adjust sprite coordinates and dimensions in:

pixelracing/images/sprites.js

Ensure changes match the pixel-art grid for visual consistency.

 Development Notes

No build tools or frameworks required.

Fully self-contained project.

Open browser DevTools for debugging:

Console logs

Network requests

Audio/media loading

Touch logic is isolated in touch.js for easy extension.

Enjoy racing!
