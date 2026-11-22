# Ester Karm Photography — website

A simple, fast, image-led website. It is made of plain HTML, CSS and JavaScript, so there is nothing to install and no account needed to edit it.

## How to view it on your Mac

**Easiest way:** double-click `index.html`. It will open in your web browser.

**Better way (closer to the real website):**

1. Open the app **Terminal** (Applications → Utilities → Terminal).
2. Type `cd ` (with a space after it), then drag the folder `Ester-Photography-Website` into the Terminal window and press Return.
3. Copy and paste this command, then press Return:

   ```
   ruby -run -e httpd . -p 8000
   ```

4. Open your browser and go to `http://localhost:8000`.

To stop the preview, go back to Terminal and press Control + C.

## What is in each folder

```
Ester-Photography-Website/
├── index.html          Home page
├── portfolio.html      All four galleries
├── about.html          About page
├── services.html       Services page
├── contact.html        Contact details
├── assets/
│   ├── css/
│   │   └── style.css   All colours, fonts, spacing and layout
│   ├── js/
│   │   └── main.js     Menu, scroll header and gentle image reveals
│   └── images/         All photographs and logos
└── README.md           This file
```

## How to replace the photographs

The images currently in `assets/images/` were taken from your existing esterkarm.com website. They are here as **starter images** so the site looks complete. Replace them with the final photographs you want to use.

1. Export your photograph as a JPG.
2. Put it in `assets/images/`.
3. Use one of these simple filenames so you do not need to edit the HTML:
   - `hero.jpg` — large portrait on the home page (1400 × 2100 px)
   - `portrait-01.jpg` to `portrait-08.jpg` — portraits (1400 × 2100 px)
   - `family-01.jpg` (1400 × 2100 px), `family-02.jpg` (1600 × 1067 px)
   - `wedding-01.jpg` (1400 × 2100 px), `wedding-02.jpg` (1600 × 1067 px)
   - `personal-01.jpg` to `personal-06.jpg` — personal stories
   - `studio-01.jpg` and `studio-02.jpg` — about page
4. Keep filenames lowercase, with no spaces. Use hyphens instead.

If you want a different filename, open the relevant `.html` file, find the old name and replace it with your new one.

For best results, keep images around 200–400 KB each. Large files slow the website down.

## How to edit the words

Open a page such as `index.html` in **TextEdit**. If the text looks formatted, choose **Format → Make Plain Text** (or press Command + Shift + T) before saving. A free editor such as Visual Studio Code is also a good option.

Text you should personalise is marked with square brackets, for example:

```
[your@email.com]
[Write a few sentences here...]
[Add your pricing details here.]
```

Search for `[` in each HTML file to find every placeholder. Replace the placeholder, keep the surrounding tags, then save.

The social links (Instagram and Facebook) are already set to your existing accounts. Search for `instagram.com` if you need to change them.

## How to change colours and fonts

Open `assets/css/style.css`. The first block, `:root`, contains the main settings:

- `--paper`: page background (currently white `#ffffff`)
- `--ink`: main text colour (black)
- `--muted`: quiet grey text
- `--line`: hairline borders
- `--accent`: the burnt orange detail colour `#c74300`, taken from your current website
- `--serif`: Cormorant Garamond, the main typeface
- `--sans`: the small uppercase labels

Change a value there and it updates across the whole site.

## How to publish it

This is a static website, so it can be published almost anywhere.

The simplest option is Netlify:

1. Create a free Netlify account.
2. Drag the entire `Ester-Photography-Website` folder onto the Netlify Deploy page.
3. Netlify will give you a live web address.
4. In your account settings you can connect your own domain name.

You can also upload the same folder to GitHub Pages, Cloudflare Pages or any normal web hosting. Do not change the folder names `assets`, `css`, `js` or `images` unless you also update the links in the HTML files.

## Notes

- All pages share the same navigation menu. To rename a menu item, change it in all five HTML files.
- The menu works on phones and tablets without any extra setup.
- The website respects visitors who prefer reduced motion.
- No prices, biography facts or contact details have been invented — everything personal is a clearly marked placeholder.
