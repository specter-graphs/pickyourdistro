# Pick Your Distro

Static guides for picking, verifying and flashing open source Linux distros. Plain HTML and CSS, no build step, no dependencies.

This site does not host operating system images. Every guide links to each project's official download page.

## Deploy on GitHub Pages

1. Create a new repository, for example `pickyourdistro`, under your GitHub account or the `specter-graphs` org.
2. Upload the contents of this folder to the root of the repository, including the hidden `.nojekyll` file.
3. Go to **Settings, Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose `main` and `/ (root)`, then save.
4. After a minute or two the site is live at `https://<owner>.github.io/<repo>/`.

All links are relative, so the site works whether it is served from a project URL or a custom domain.

## Add a new post

1. Copy any file in `posts/` and rename it, for example `posts/dual-boot-safely.html`.
2. Edit the title, description, date and body.
3. Add a header image (1200x630 works well) to `assets/images/` and update the `<img>` and `og:image` paths.
4. Add a card for it in `index.html`, and update the previous and next links at the bottom of neighbouring posts.

## Custom domain (optional)

Add a file called `CNAME` containing your domain, such as `pickyourdistro.example.com`, then set the same domain in **Settings, Pages**.

## Structure

```
index.html
style.css
.nojekyll
posts/
  lightweight-distro.html
  verify-sha256.html
  bootable-usb.html
assets/images/
  lightweight-distro.png
  verify-sha256.png
  bootable-usb.png
```
