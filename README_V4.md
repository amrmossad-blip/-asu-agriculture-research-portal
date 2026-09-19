ASU Agriculture Research Portal V4 – Professional Review Workflow

Upload/replace BOTH files in the ROOT of the existing GitHub repository:
1) index.html
2) admin.html

Do not delete other repository files.

Researcher portal:
https://amrmossad-blip.github.io/-asu-agriculture-research-portal/

Admin:
https://amrmossad-blip.github.io/-asu-agriculture-research-portal/admin.html

Implemented:
- Expanded candidate publication matching across the current publication corpus.
- Research progress: reviewed / pending / complete.
- Explicit confirmation when no publications are found, or when all candidates are marked Not Mine.
- Admin dashboard review-status metrics.
- Full/changes Excel export now includes researcher review status.
- Login attempt rate limiting.
- CORS restricted to the GitHub Pages origin.
- Email OTP backend prepared as Supabase Edge Function `portal-email-auth`.

Email OTP is intentionally NOT shown in the UI yet because a trusted sending provider must be configured first.
Required Supabase secrets for Resend:
- RESEND_API_KEY
- PORTAL_FROM_EMAIL
- optional: PORTAL_FROM_NAME

After those are configured and the sender domain is verified, the portal can switch from permanent access codes to one-time email codes.
