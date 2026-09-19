# ASU Agriculture Research Portal — GitHub + Render Frontend

واجهة Pilot مستقلة لمنصة توثيق أبحاث كلية الزراعة — جامعة عين شمس.

## Architecture

- **GitHub**: source control for this frontend.
- **Render Static Site**: serves `index.html` over HTTPS.
- **Supabase**: existing database, Storage and `portal-api` backend.

This package intentionally does **not** contain database passwords, service-role keys, researcher access codes, or other secrets.

## Current backend

The frontend calls the existing Supabase Edge Function:

`https://xaddbgzrnhaixkqrotkz.supabase.co/functions/v1/portal-api`

The API endpoint is configured in `config.js`.

## Render deployment

Recommended settings:

- Service type: **Static Site**
- Repository: the GitHub repository containing these files
- Branch: `main`
- Build command: `echo "No build required - static portal"`
- Publish directory: `.`
- Auto deploy: enabled

Alternatively, Render can read the included `render.yaml` as a Blueprint.

## Important

Do not add Supabase secret/service-role keys to this repository or to browser JavaScript.
The current browser frontend talks only to the server-side `portal-api`.

## Pilot

Only researchers whose portal access is `Pilot Enabled` or `Active` can log in through the current backend.
