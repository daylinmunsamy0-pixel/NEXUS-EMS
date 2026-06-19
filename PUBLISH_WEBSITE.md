# Publish NEXUS EMS

The public website build is in `web/`.

Use any static website host that serves `index.html` as `text/html`, for example:

- Netlify: drag the `web` folder into Netlify Drop.
- Vercel: create a static project with `web` as the output/publish folder.
- Cloudflare Pages: upload the `web` folder as direct upload.
- GitHub Pages: publish `web/index.html` from a repository.

Supabase should remain the database. Do not use Supabase Edge Functions or Supabase Storage as the website host for this HTML app because those gateways serve HTML as `text/plain` with a sandbox policy.

After editing `LIMAS V2.HTML`, copy it to `web/index.html` again before redeploying.
