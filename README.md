# Samskrita Bharati New Zealand - website

This is the SBNZ website. It is built with [Jekyll](https://jekylljs.org) and
hosted free on GitHub Pages. You do not need to install anything to edit it -
everything can be done through the GitHub website in a browser.

---

## The five things you will actually do

### 1. Add or change an event
Open `_data/events.yml`, copy an existing four-line block, and change the
month, day, title, and detail. Save (commit). The site updates in about a
minute.

### 2. Write a blog post
Copy the file in `_posts/`, rename it with today's date at the front
(`YYYY-MM-DD-a-short-title.md`), change the title and date at the top, write
your post below the second `---`, and commit.

### 3. Edit a page's words
Open the page file (`about.md`, `contact.md`, `learn.html`, etc.), change the
text, and commit.

### 4. Change the class levels
Edit `_data/classes.yml`. The Learn page rebuilds itself from this file.

### 5. Add or hide a page
There is a ready-made spare page at `spare.md`. See the notes inside it for how
to publish it (add it to the menu in `_config.yml`) or hide it completely
(`published: false`).

---

## How the site is put together

| Folder / file        | What it is                                             |
|----------------------|--------------------------------------------------------|
| `_config.yml`        | Site title, menu, contact email, settings              |
| `index.html`         | The home page                                          |
| `about.md` etc.      | The other pages                                         |
| `_data/`             | Events and class lists (the files you edit most)       |
| `_posts/`            | Blog posts                                             |
| `_layouts/`          | Page templates (rarely need changing)                  |
| `_includes/`         | Header, footer, event card (rarely need changing)      |
| `assets/css/`        | The single stylesheet - all colours are at the top     |
| `assets/images/`     | Put photographs and images here                        |

## Changing the look
All colours and fonts live at the very top of `assets/css/style.scss`, in the
`:root` block. Change a value there and the whole site follows.

---

## Publishing (one-time setup)

1. Create a **GitHub organisation** for SBNZ (free) so the site belongs to the
   group, not to one person. Each committee member signs in with their own
   GitHub account - no shared passwords.
2. Create a **repository** in that organisation and upload these files.
3. In the repository, go to **Settings > Pages** and set the source to the
   `main` branch. GitHub gives you a free web address to test on.
4. When you are ready to use your own domain, add it under **Settings > Pages >
   Custom domain**, and point the domain's DNS at GitHub Pages.

## Previewing on your own computer (optional)
Only if you want to. With Ruby installed:

    bundle install
    bundle exec jekyll serve

then open <http://localhost:4000>.
