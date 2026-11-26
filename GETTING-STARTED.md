# A short guide to your site

Hi Abby — this is a plain-language walkthrough of the files behind [abbyodell.com](https://abbyodell.com), and how to make your first change. You don’t need any special software. Everything here can be done in a web browser.

The site is a simple “coming soon” page for now. Later it will become your film résumé and portfolio.

## How a folder on GitHub becomes abbyodell.com

Think of this repository (or “repo”) as a shared folder that holds every file for your site. It’s at [github.com/paulkodell/abbyodell-site](https://github.com/paulkodell/abbyodell-site).

GitHub Pages is the free service that turns that folder into a website. Whenever someone saves a change to the `main` branch, GitHub republishes the site. It usually takes about a minute.

Two other pieces make the address `abbyodell.com` work:

- A tiny file in this repo named `CNAME`. It tells GitHub, “this site’s public name is abbyodell.com.” **Please leave this file alone.** Changing it can take the domain offline.
- DNS records at GoDaddy, where the domain was registered. Those records point abbyodell.com at GitHub, the same way a contact card points a name at a phone number. You don’t need to touch those either.

`www.abbyodell.com` automatically sends people to [abbyodell.com](https://abbyodell.com).

## What’s in the folder

| File | What it does |
| --- | --- |
| `index.html` | The actual page people see. Your name, the tagline, and the look of the page all live here. This is the file you’ll edit. |
| `README.md` | A short description of the project. It shows at the bottom of the repo’s main GitHub page. |
| `CNAME` | The “this site is abbyodell.com” note described above. Don’t edit it. |
| `GETTING-STARTED.md` | This guide. |

There’s also a `.gitignore` file, which just tells Git to skip a couple of leftover local files. You can ignore it.

## Your first edit, right on the GitHub website

Let’s change the tagline. That’s the line under your name that currently says “Film student & film archivist — portfolio and resume coming soon.”

1. Open the repo: [github.com/paulkodell/abbyodell-site](https://github.com/paulkodell/abbyodell-site).
2. Click **index.html**.
3. Click the pencil icon in the toolbar (it may say “Edit this file”).
4. Find this line:

   ```html
   <p class="line">Film student &amp; film archivist — portfolio and resume coming soon</p>
   ```

5. Change only the words between `>` and `</p>`. For example:

   ```html
   <p class="line">Film student &amp; film archivist — a portfolio is on the way</p>
   ```

6. Scroll to the bottom of the page. Leave **Commit directly to the `main` branch** selected. Type a short note such as “Update the tagline,” then click **Commit changes**.
7. Wait about a minute, then refresh [abbyodell.com](https://abbyodell.com). If you don’t see the change yet, give it another moment and refresh again.

That’s it. A “commit” is just a saved snapshot with a short message, like a labeled version of the file.

## If something looks wrong

Nothing is permanent. Every save is kept in the repo’s history, so you can always go back.

The simplest fix is to copy an older version back in:

1. Open **index.html**, then click **History** (sometimes labeled “Blame” is next to it — you want History).
2. Click an earlier commit that still looks right.
3. Click the file name to see that older version, copy the text, go back to Edit, paste it in, and commit to `main` again.

You can also open the **Commits** list on the repo, click a change you want to undo, and use **Revert**. That creates a new save that puts things back, without erasing the history.

If you’re unsure, stop and ask. It’s much easier to undo a change than it looks.

## A tiny bit of HTML

HTML is just text with labels that tell the browser what each part is. You only need a few of those labels for this page.

- `<h1>Abby O’Dell</h1>` is the big heading — your name.
- `<p class="line">…</p>` is the tagline under your name. The words you’ll change sit between those two tags.
- In HTML, an ampersand has to be written as `&amp;` (that’s why the line says `Film student &amp; film archivist` even though the page shows “Film student & film archivist”). A regular `&` can break the page, so keep `&amp;` if you still want an “and” symbol.
- The big `<style>…</style>` block near the top is the look of the page: the dark background, the film-strip edges, the fonts. You can leave that alone for now.

If a tag is opened, it should be closed. If you delete a `<p>` or `</p>` by accident, the page can look strange until that’s put back.

## What’s coming next

This coming-soon page is a placeholder. The real site will be your résumé and portfolio: your film and archival work, reel links, and stills.

When you’re ready to build that out, send along a résumé, reel links, and any project stills you’re happy to show, and we’ll turn this into the real site — still at the same address, abbyodell.com.

Welcome in. Change the tagline when you feel like it, and don’t worry about experimenting.
