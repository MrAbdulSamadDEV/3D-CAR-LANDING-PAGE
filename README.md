# VANTA — Scroll-Driven Car Landing Page

A cinematic, responsive automotive landing-page concept. The car sequence is made from numbered JPG frames and is controlled by the visitor’s scroll position: scroll down to move forward through the sequence, and scroll up to move backward.

## Features

- **Scroll-controlled animation** using an HTML canvas and a numbered JPG image sequence.
- **75 JPG frames**, loaded from the local `frames/` folder.
- **Responsive layout** for desktop and smaller screens.
- **Cinematic sections** for the hero, design details, experience, and closing call to action.
- **Social and portfolio links** in the footer: GitHub, personal portfolio, LinkedIn, YouTube, X, and Instagram.
- **Loading indicator** while the frame sequence is being prepared.
- Built with plain **HTML, CSS, and JavaScript** — no framework or package installation required.

## Quick Start

1. Download and extract the ZIP file.
2. Open the extracted `car-scroll-hd-jpg` folder.
3. Make sure `index.html` and the `frames` folder remain together. Do not move or rename individual frame files.
4. Open `index.html` in a modern browser such as Google Chrome or Microsoft Edge.
5. Wait for the frame-loading indicator to finish, then scroll through the hero section to control the car sequence.

> **Important:** Keep the folder structure intact. The page expects files named `frames/frame_0001.jpg` through `frames/frame_0075.jpg`.

### If images do not appear

Some browsers may restrict local-file behavior in certain setups. If the page opens but the frames do not load, run a small local web server from inside the extracted project folder instead of opening the file directly. If Python is installed, open a terminal in that folder and run:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000` in your browser. On some Windows systems, the command may be `py -m http.server 8000`.

## Project Structure

```text
car-scroll-hd-jpg/
├── index.html       # Page layout, styles, and animation logic
├── README.md        # This guide
├── README.txt       # Short setup note
└── frames/
    ├── frame_0001.jpg
    ├── frame_0002.jpg
    ├── ...
    └── frame_0075.jpg
```

## Customize Your Links

The footer links are inside `index.html`. Search for `CONNECT WITH ME` and update the corresponding `href` values if you want to change a profile URL. The current links are:

- GitHub: https://github.com/MrAbdulSamadDEV
- Portfolio: https://samad.vexr.dev
- LinkedIn: https://www.linkedin.com/in/MRABDULSAMADDEV
- YouTube: https://www.youtube.com/@epicflixplus
- X: https://x.com/ABDULSAMAD8492
- Instagram: https://www.instagram.com/samad_boy.dev

## Image Quality Note

The frames in this package have been upscaled for display to **1472 × 828**. The source images were **736 × 414**, so upscaling increases pixel dimensions but cannot recover original fine detail or create true native 1080p/4K footage. For the sharpest result, use higher-resolution source frames.

## Performance Notes

- The page preloads the image sequence and draws the relevant frame to a canvas as the page scrolls.
- First load can take a little time because all frames are local image assets.
- For best performance, use a modern browser and avoid deleting frames from the `frames/` folder.
- If you replace the images, keep the same file names and dimensions where possible. If you change the number of frames, update the `count` value in the JavaScript and the frame totals displayed in the HTML.

## Credits and License

This is a personal landing-page concept. Make sure you have the rights to use and redistribute the car images and any other assets included in your own published version. No third-party framework is required by this project.
