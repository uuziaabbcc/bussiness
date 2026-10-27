# yuanfanzhituo Marketing Website

A responsive, English-language static HTML/CSS website inspired by the four-page structure and teal/copper palette of yuanfanzhituo.com. No dependencies or build step are required.

## Products and contact information

The site uses the `yuanfanzhituo` brand. Product information and icons were checked against the following App Store listings and public Apple Lookup data on October 27, 2026:

- [Pennyline Expense Tracker](https://apps.apple.com/cn/app/pennyline-expense-tracker/id6803852051): local income and expense records, category search, and monthly summaries.
- [MemoNest Quick Notes](https://apps.apple.com/cn/app/memonest-quick-notes/id6806918110): local notes, search, and pinning.
- [NestTick](https://apps.apple.com/cn/app/nesttick/id6806914937): task lists, due dates, and priorities.

Contact addresses retain the exact spelling supplied by the owner:

- Technical Support: `support@yuanfanzhituo.com`
- Business Support: `contact@yuanfanzhituo.com`
- Key Accounts: `dongdong@yuanfanzhituo.com`
- Email: `bussion@yuanfanzhituo.com`

Email links open the device's email application. The website does not store or submit form data. No unverified registered company name, address, or credentials have been added.

## Local preview

Run from this directory:

```sh
python3 -m http.server 4173
```

Open `http://localhost:4173`.

## GitHub → Vercel

### Recommended: a separate repository

1. Create a GitHub repository, such as `app-marketing-site`.
2. Upload the files in this directory, including `assets`, with `index.html` at the repository root.
3. In Vercel, choose **Add New → Project → Import Git Repository** and select the repository.
4. Select **Other** as the Framework Preset and keep the repository root as the Root Directory.
5. Leave the build and install commands unset. The output directory is `.`; `vercel.json` includes these settings.
6. Use the production address assigned by Vercel, such as `https://project-name.vercel.app`.

Later pushes to the connected production branch trigger automatic deployments.

### Using the existing monorepo

If you import the repository containing this directory, set Vercel's **Root Directory** to `marketing-site`, rather than the pi-main repository root.

## Pages

| Path | Content |
| --- | --- |
| `/` | Home: brand, app overview, and support links |
| `/services.html` | Products & Services: brief app descriptions, App Store links, and support channels |
| `/technology.html` | Technical Strength: local records, organization, search, and usability |
| `/contact.html` | Contact Us: four email channels and feedback guidance |
| `/support.html` | Product Support and frequently asked questions |
| `/privacy.html` | Website privacy notice and App Store privacy information links |
| `/terms.html` | Website terms of use |

After deployment, the home page or `/services.html` can serve as the marketing URL. Use `/support.html` or `/contact.html` as the support URL. The website notice at `privacy.html` does not replace an app's privacy policy.

## Visual assets

The three JPG app icons come from their corresponding public App Store assets. `assets/hero.svg`, `assets/workspace.svg`, and `assets/mark.svg` were created for this site. All assets are stored locally; the pages do not depend on external image, script, or font services.
