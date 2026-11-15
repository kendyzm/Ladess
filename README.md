# Music Enthusiasts

Static GitHub Pages site for hip-hop videos and original music-culture articles.

## Pages
- `index.html` — homepage with latest three videos and article features.
- `all-videos.html` — complete video archive.
- `all-articles.html` — article index.
- `videos/` — individual YouTube embed pages.
- `articles/` — original editorial article pages with source links.
- `assets/style.css` — site styles.

## Publish
Upload all files and folders to the root of your GitHub repository. In **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.

## Video ordering
The homepage sorts video cards by `data-date` values (YYYY-MM-DD). Enter each video's verified YouTube public publish date. Dates are not guessed. Undated entries remain in the fallback order. The homepage displays three cards; the full archive is available from **View all videos**.

To add a video, create its individual page in `videos/`, add its card to `index.html` and `all-videos.html`, and set its verified `data-date`.

Article copy is original editorial writing based on source reporting, with a link and credit to the original publication. Check source links for updates.
