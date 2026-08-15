# Sergii Drobot — Academic Website

This is a simple static academic website inspired by the Minimal Light layout. It does not require Jekyll, Ruby, or a build process.

## Local preview

Double-click `index.html`, or run this command inside the website folder:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Publish with GitHub Pages

1. Create a public GitHub repository named `YOUR-USERNAME.github.io`.
2. Upload all files and folders from this package to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then save.
6. The site will be available at `https://YOUR-USERNAME.github.io`.

## Essential edits

### Add a profile photograph

Save the image as `assets/img/profile.jpg`. In `index.html`, replace the initials placeholder with the commented `<img>` line immediately below it.

### Add the CV

Save the CV as `assets/files/Sergii_Drobot_CV.pdf`. The CV icon is already configured.

### Activate Google Scholar and LinkedIn

In `index.html`, replace the default Google Scholar URL with your profile URL. For LinkedIn, replace `href="#"` with your profile URL, then remove `class="disabled"` and `aria-disabled="true"`. The icons use Academicons and Font Awesome through CDN links in the page header, so an internet connection is needed for them to appear.

### Add news

Inside the `<section id="news">` list, copy this format:

```html
<li><span class="news-date">Month Year</span> Your update, seminar, or conference.</li>
```

### Add papers

Save PDFs with these filenames:

- `assets/files/news-sentiment-inflation-expectations.pdf`
- `assets/files/incentivizing-inflation-expectations.pdf`
- `assets/files/choosing-digital-currency-design.pdf`

To link a paper to SSRN instead, replace its local PDF path in `index.html` with the full SSRN URL and change the button text from `View PDF` to `View on SSRN`.

### Add presentations

Replace the text after `<strong>Presented at:</strong>` under each paper with the relevant conferences, workshops, and seminars.
