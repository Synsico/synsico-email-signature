# Synsico Analytics - Email Signature

Personalized animated email signature for Shaquille Johnson.

**Project status:** Prepared for GitHub Pages. This package does not create a repository, publish a website, or change an email account. No GitHub account or repository URL has been assumed.

## Contact details

```text
Shaquille Johnson
AI Manager | Consultant
SYNSICO ANALYTICS
Systems for a Smarter World.

Shaquille@synsico.com
(813) 530-5117
https://www.Synsico.com

7901 4th St N #31272
St. Petersburg, FL 33702, USA
```

The phone link is `tel:+18135305117`. Email, website, and contact-rail icons are clickable in the HTML and email-draft exports. The supplied website spelling is preserved in visible text; browsers normalize the website link hostname.

## Publish with GitHub Pages

Use a separate repository named `synsico-email-signature` so the company website is not replaced. No custom domain or `CNAME` file is included.

1. Create the repository in the intended GitHub account or organization. GitHub Free requires a public repository for Pages. Upload the extracted package contents to the `main` branch: `index.html`, the `assets` folder, and the other supplied files. Do not upload only the ZIP and do not place `index.html` inside an extra enclosing directory.
2. In the repository, open **Settings > Pages**. Under **Build and deployment**, choose **Deploy from a branch**, select **main** and **/(root)**, then **Save**. The branch must already exist, and the account needs permission to configure Pages. When the Settings tab is hidden, check the repository's navigation overflow menu.
3. After deployment succeeds, use **Visit site** in Pages settings. The usual project URL is shown below; replace the placeholder with the actual account or organization. A custom domain already configured for the account may change the final URL, so use the address GitHub actually displays.

```text
https://YOUR-GITHUB-USERNAME.github.io/synsico-email-signature/
```

Official GitHub documentation:

- https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages

Publishing exposes the supplied business contact details and image files publicly. The `noindex` meta tag is a search-crawler request, not an access-control mechanism. There are no credentials, customer records, analytics scripts, or tracking pixels in this project.

## Use the hosted signature

Open the published HTTPS page. The editor automatically derives its public `assets/` URL. Use **Copy signature**, paste into your email application's signature settings, save, and send yourself a test email.

The formatted copy contains ordinary text, hyperlinks, a presentation table, and HTTPS image references. It does not include the editor's JavaScript. Do not paste the editor source into an email. The full-card GIF and PNG are previews, not substitutes for the clickable HTML signature.

**Save email HTML** exports an email-only HTML file with public image URLs. **Save email draft** exports an unsent `.eml` with inline image attachments and no recipient; it does not require image hosting. The included `synsico-signature.eml` is already personalized. **Copy plain text** provides an image-free alternative. Switch Animation off before exporting to use the static artwork.

No account signature is installed automatically. Keep the hosted image filenames and URLs stable for previously sent emails. Test the final result in the email applications you use; rendering, pasted images, and animation depend on the application and its settings. This package has not been sent through Gmail or Outlook for end-to-end testing.

## Files

```text
index.html                 Self-contained editor and Pages entry point
signature.html             Email-only animated HTML with relative asset paths
signature-static.html      Email-only static HTML with relative asset paths
signature.txt              Personalized plain-text signature
signature-settings.json    Reference copy of the prefilled profile
synsico-signature.eml       Personalized unsent draft with embedded images
signature-preview.png      Updated full-card static preview
signature-preview.gif      Updated full-card animated preview
assets/                    Mark, icons, animation, and static artwork
.nojekyll                  Publish the supplied static files without Jekyll
```

`index.html` includes embedded artwork for offline preview. The separate `assets` folder is still required on the published site because the email exports reference its public image URLs.

The HTML email files use the original fixed 660-pixel layout. The editor scales its preview on small screens; that scaling is not a guarantee about every email client's layout.

## Editing the code

Temporary edits in the browser affect the current preview and exports only. They are not saved to GitHub. To change the initial profile in code, edit the `DEFAULTS` object in `index.html`, then commit that change. `signature-settings.json` is a reference copy, not a dynamically loaded configuration file. Update the email-only files and full-card previews when publishing a revised static profile.

There is no build step, package manager, server-side application, or environment-variable configuration. Everything served is static HTML or an image. The page makes no application API calls.
