# Apex Edge Lawn Care — Website

A one-page site for Apex Edge Lawn Care. Plain HTML, CSS, and a little
JavaScript. No build step. No frameworks. It runs anywhere.

## Files

- `index.html` — the whole site
- `assets/` — logo, favicon, and social image

## Put it online with GitHub Pages (free)

1. Make a new repository on GitHub.
2. Upload `index.html` and the `assets` folder to it.
3. In the repo, go to **Settings → Pages**.
4. Under **Branch**, pick `main` and the `/ (root)` folder. Save.
5. Wait a minute. Your site shows up at
   `https://YOURNAME.github.io/REPONAME/`.

Want a custom name like `apexedgelawn.com`? Buy the domain, then add it
under **Settings → Pages → Custom domain**.

## How the quote form works

Right now, when someone fills out the form and hits send, it opens their
email app with the details filled in, addressed to apexedgekc@gmail.com.
This works out of the box. It needs no account and no setup.

The catch: it depends on the visitor having an email app set up.

### Better option: have quotes land in your inbox automatically

Use Formspree. It is free for a small number of monthly quotes.

1. Sign up at https://formspree.io with apexedgekc@gmail.com.
2. Create a form. Copy the form's web address. It looks like
   `https://formspree.io/f/abcwxyz`.
3. Open `index.html` and find the line that starts with
   `<form class="quote-form"`.
4. Change it so it reads:

   ```html
   <form class="quote-form reveal" id="quoteForm" method="POST" action="https://formspree.io/f/abcwxyz">
   ```

   Use your own address from step 2. Also delete the part that says
   `onsubmit="return sendQuote(event)"`.
5. Save and re-upload. Done. Quotes now arrive in your Gmail.

## Editing the site

- Phone, email, and city all sit in plain text in `index.html`. Search for
  the old value and type the new one.
- Service area towns are in the section marked `id="area"`.
- To add a service later, copy one of the two service cards in the
  section marked `id="services"` and change the words.

## Colors

- Green: `#4B5D2F`
- Tan: `#BA9765`
- Cream background: `#FBFAF3`
