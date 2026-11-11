# CJKmap landing page

Static Vite site prepared for Cloudflare Pages.

## Local development

Requires Node.js 20.19+ or 22.12+.

```sh
npm install
npm run dev
```

## Production build

```sh
npm run build
npm run preview
```

Vite writes the deployable static site to `dist/`.

## Deploy to Cloudflare Pages

1. Push this project to a GitHub or GitLab repository.
2. In Cloudflare, choose **Workers & Pages → Create → Pages → Connect to Git**.
3. Use these build settings:
   - Build command: `npm run build`
   - Build output directory: `dist`
   - Root directory: `/`
4. Deploy. Subsequent pushes to the production branch deploy automatically; other branches get preview deployments.

This landing page is static and needs no Workers, database, or environment variables.

The page includes a title, description, social sharing metadata, structured data, a favicon, and `robots.txt`. Once a production domain is attached, add its canonical URL and sitemap URL to the page; they are intentionally omitted until the domain is known.
