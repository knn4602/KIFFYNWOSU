# Kiffy OS

Kifekachukwu Nwosu's portfolio: a riso-printed desktop where each folder opens a zine-style window. Built with plain HTML, CSS and JavaScript, so there's no build step and nothing to install.

## What's in this folder

```
kiffy-os/
├── index.html          ← the whole site (content, styles and scripts)
├── README.md           ← this guide
└── assets/
    ├── photos/         ← headshot and travel/event photos
    ├── recordings/     ← short screen recordings of your projects (.mp4)
    └── resumes/        ← your three résumé PDFs (already added)
```

## Preview it

Double-click `index.html` to open it in your browser. Every time you save a change, refresh the page.

For live reloading, open the folder in VS Code and install the **Live Server** extension, then click **Go Live**.

## Fill it in

1. Open `index.html` in VS Code.
2. Search (Ctrl+F or Cmd+F) for **`EDIT`**. Every spot to fill in is marked `[EDIT: ...]`, and it shows on the page as pink dashed text.
3. Replace the text inside the brackets and delete the brackets.

Each folder is one block that starts with a banner comment like this:

```html
<!-- ===================================== EVENTS ===================================== -->
```

### Adding your photo

Name your photo **headshot.jpg** and put it in `assets/photos/`. That's it: it shows up automatically in the big About card on the home screen and in the About window. No code changes needed.

On GitHub: open the `assets` folder, then `photos`, click **Add file → Upload files**, drop in `headshot.jpg` and commit.

### Adding a screen recording

1. Record a short clip (10–30 seconds) of the project running and save it as an .mp4 in `assets/recordings/`, for example `heartstrings.mp4`.
2. In the CODE section, replace the `<span>[EDIT: ...recording]</span>` inside that project's `<div class="demo">` with

```html
<video src="assets/recordings/heartstrings.mp4" autoplay muted loop playsinline aria-label="HeartStrings demo"></video>
```

Keep clips small (under about 10 MB each) so the site loads fast.

### Laptop stickers

The details that appear when someone taps a laptop sticker are in the `skills` list near the bottom of `index.html`.

### The home screen collage

The clickable objects on the desktop (polaroid, laptop, badge, magazine, photo, award) are in the `collage` block near the top of `index.html`. When you add your headshot, also replace `<span class="hi">hi, I'm Kiffy!</span>` inside the polaroid with `<img src="assets/photos/headshot.jpg" alt="">`.


### Adding a new entry

Copy an existing `<article class="entry" ...> ... </article>` block in the same folder, paste it below, and change the text.

## Put it online with GitHub Pages

1. Create a GitHub account if you don't have one.
2. Create a new **public** repository named exactly `YOUR-USERNAME.github.io`.
3. Click **Add file → Upload files**, drag in everything inside this folder (index.html, README.md and the assets folder), and click **Commit changes**.
4. Go to **Settings → Pages**. Under **Branch**, choose `main` and `/ (root)`, then click **Save**.
5. After a minute or two, your site is live at `https://YOUR-USERNAME.github.io`.

To update the site later, upload the changed files again (or use Git), and GitHub Pages republishes automatically.

### Optional: your own domain

Buy a domain (for example `kifekachukwu.com`, about $10–15 a year), then add it under **Settings → Pages → Custom domain** and follow GitHub's DNS instructions.

## Before you publish: checklist

- [ ] No `[EDIT` left (search the file)
- [ ] Headshot added
- [ ] LinkedIn and GitHub links in Contact
- [ ] At least one screen recording in Code
- [ ] Conference names and dates
- [ ] Event details on the flyer wall
- [ ] Leadership platform and achievements
- [ ] Open it on your phone to check the scroll view
