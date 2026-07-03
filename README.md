# David Besin — Portfolio

A minimal, static portfolio site. No build step, no dependencies — just `index.html`, `style.css`, and `script.js`.

## Host it on GitHub Pages (free)

1. **Create a repository.** On GitHub, click **New repository**. Name it whatever you like — if you name it exactly `yourusername.github.io`, your site will live at the root of your GitHub domain instead of a subpath.

2. **Upload the files.** Either drag `index.html`, `style.css`, and `script.js` into the repo via the GitHub web UI, or push from your machine:
   ```bash
   git init
   git add index.html style.css script.js
   git commit -m "Add portfolio site"
   git branch -M main
   git remote add origin https://github.com/yourusername/your-repo.git
   git push -u origin main
   ```

3. **Turn on Pages.** In the repo, go to **Settings → Pages**. Under **Build and deployment → Source**, choose **Deploy from a branch**. Under **Branch**, pick `main` and `/ (root)`, then **Save**.

4. **Wait a minute, then visit your site.** GitHub will show the live URL at the top of the Pages settings once it's built — usually:
   - `https://yourusername.github.io/your-repo/` (normal repo name), or
   - `https://yourusername.github.io/` (if you named the repo `yourusername.github.io`)

Any time you push a change to `main`, the live site updates automatically within a minute or two.

## Adding more projects later

Copy one `<article class="project-card">...</article>` block in `index.html`, swap the image, title, description, and the `<dl class="inspector">` rows (Status, Platform, Made with, Genre, Role) to match your new project, and update the link.
