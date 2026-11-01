# Policy site (GitHub Pages)

Static pages used as the public home, privacy policy, and terms of service for
DT Summary Bot. No build step or dependencies — plain HTML and one stylesheet.

| File | Purpose |
| --- | --- |
| `index.html` | Home page (app description, Google data usage, contact) |
| `privacy.html` | Privacy policy, including the Google API Limited Use disclosure |
| `terms.html` | Terms of service |
| `404.html` | Not-found page |
| `assets/style.css` | Shared styles (light/dark, responsive, print) |
| `assets/favicon.svg` | Favicon |
| `.nojekyll` | Serve files as-is, without Jekyll processing |

## Publish with GitHub Pages

1. Push this repository to GitHub.
2. Open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select branch **main** and folder **/docs**, then save.
5. After the first deployment, the site is available at
   `https://<username>.github.io/<repository>/`.

For this repository that is:

- Home: https://deltatiger.github.io/dt-summary-bot/
- Privacy: https://deltatiger.github.io/dt-summary-bot/privacy.html
- Terms: https://deltatiger.github.io/dt-summary-bot/terms.html

All links are relative, so the site also works on a user/org Pages site or a
custom domain.

## Google OAuth consent screen

Use the published URLs in **Google Cloud Console → APIs & Services → OAuth consent
screen**:

- **Application home page**: the Home URL above
- **Privacy policy**: the Privacy URL above
- **Terms of service**: the Terms URL above
- **Authorized domain**: `deltatiger.github.io`

Keep the contact address in the pages (`deltatiger94@gmail.com`) in sync with the
support email configured on the consent screen.

## Editing

- Update the effective/last-updated dates in `privacy.html` and `terms.html` when
  their content changes.
- If the app's data handling changes (new provider, new scope, new storage), update
  `privacy.html` and the summary table on `index.html`.
