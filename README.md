# Filmmaker portfolio

A responsive navy and white portfolio for film projects, production credits, photos and videos.

## Website

The public site is at https://fuaddd06.github.io/portfolio/.

## Preview on your computer

1. Install Node.js LTS from https://nodejs.org/.
2. Open PowerShell in the portfolio folder.
3. Run npm run dev and keep that window open.
4. Visit http://localhost:4173/ in your browser.

## Add and edit content

Edit content/portfolio.js to change your introduction, experience, education, languages, software, project descriptions, dates, roles, and video links. The three films marked as your own are listed first, with Something Good at the top.

Add your portrait as media/portrait.jpg. Put a project's cover and stills in its matching folder under media/projects/ (for example, media/projects/something-good/cover.jpg and still-01.jpg). JPG, PNG and WebP images work. Update the matching paths in content/portfolio.js when you use different filenames. Add another project by copying a project entry, giving it a unique slug, and creating a matching media folder. Use owned: true for your own films and set the order in the content file.

## One-time Git setup on Windows

Install Git for Windows from https://git-scm.com/download/win. Then open PowerShell in this existing portfolio folder and run these commands once:

~~~powershell
git init -b main
git remote add origin https://github.com/fuaddd06/portfolio.git
git fetch origin
git reset origin/main
git push -u origin main
~~~

On the first push, Git may open a browser so you can sign in to GitHub. The reset attaches this folder to the existing repository history and leaves your local files in place.

## Publish updates

1. Save your changes and add any new photos or videos to the media/ folders.
2. In PowerShell, run these commands:

~~~powershell
git add .
git commit -m "Update portfolio"
git push
~~~

Each push to main starts the GitHub Pages workflow. In the repository, Settings → Pages should show GitHub Actions as the publishing source. Publishing is public, so only add material you want visitors to see.