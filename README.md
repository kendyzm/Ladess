# Music Enthusiasts — Video Website

A responsive static website designed for GitHub Pages. Each video has its own HTML page and embeds the original YouTube video.

## Preview locally
Open `index.html` in a browser. For a closer match to GitHub Pages, run a simple local static server from this folder.

## Publish with GitHub Pages
1. Create a new GitHub repository (or use an existing website repository).
2. Upload the contents of this folder — make sure `index.html` is at the repository root.
3. In GitHub, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select your main branch and `/ (root)`, then Save.
6. Wait for GitHub Pages to publish the site.

## Add another video
1. Copy one of the HTML files inside `videos/` and give it a new descriptive filename.
2. Replace the YouTube video ID in the embed URL and the YouTube link.
3. Update the page title, category and description.
4. Add a new card to the `cards` section in `index.html`. Use this pattern:

```html
<article class="card">
  <a class="thumb" href="videos/your-new-video.html">
    <img src="https://i.ytimg.com/vi/YOUTUBE_VIDEO_ID/hqdefault.jpg" alt="Video title thumbnail" loading="lazy">
    <span class="play" aria-hidden="true">▶</span>
  </a>
  <div class="card-body">
    <div class="tag">Category</div>
    <h3><a href="videos/your-new-video.html">Video title</a></h3>
    <p>Short description.</p>
    <a class="card-link" href="videos/your-new-video.html">Watch video ↗</a>
  </div>
</article>
```

## Notes
- The site does not host or download YouTube videos; it embeds them from YouTube.
- Thumbnails are loaded from YouTube's public thumbnail endpoint.
- You can edit the text, colors and layout in `assets/style.css` and the HTML files.
- If a video is removed, made private, or embedding is disabled by its owner, it may not play on the site.
