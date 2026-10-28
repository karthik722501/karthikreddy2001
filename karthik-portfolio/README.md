# Karthik R — 3D Portfolio

A plain HTML/CSS/JS project. No build step, no npm, no framework.

## Run it in VS Code

1. Unzip, then in VS Code choose **File > Open Folder** and pick this folder.
2. Install the **Live Server** extension (VS Code will suggest it) and right-click `index.html` > **Open with Live Server**.
   Or just double-click `index.html` to open it in your browser.
3. You need internet for the Google Fonts only; everything else is local.

## Folder structure

```
index.html                 the whole site (HTML + CSS + JS)
assets/
  videos/
    hero-background.webm   Hero section background (with audio)
    about-background.webm  About section background (with audio)
    site-background.webm    Fixed full-page background (with audio)
  images/
    profile/               your portrait photo
    projects/              5 project infographics
    experience/            5 experience infographics
    education/             Atria (MCA) and Karnataka College (BCA)
    achievements/          UGC-NET poster
  originals/               your original full-quality files
    images/                original PNG/JPEG infographics, photo, poster
    videos/                original MP4 videos
```

## Editing tips

- **Colours**: CSS variables at the top of `index.html` under `:root` (dark) and `:root[data-theme="light"]`.
- **Projects and experience text**: the `PJ` and `EX` arrays in the `<script>` near the bottom of `index.html`.
  Each entry's last item is the image path, e.g. `assets/images/projects/banking-application.jpg`.
- **Swap a picture**: replace the file in `assets/images/...` with another file of the same name, or change the path.
- **Swap a video**: replace `assets/videos/hero-background.webm`, `about-background.webm` or `site-background.webm`.
  The files in `assets/originals/videos/` are your original MP4s. To use one, change the `<source src=...>` and `type="video/mp4"`.
- **Video sound**: browsers block autoplay with sound, so videos start muted. Use the Sound button at the bottom-right of each video.
- **Download CV link**: search `drive.google.com` in `index.html`.

## Hosting

It is a static site, so GitHub Pages, Netlify or Vercel work. Upload the whole folder (you can leave out `assets/originals`).
