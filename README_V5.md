V5 adds verified self-registration.
Only exact @agr.asu.edu.eg emails are accepted.
The user must verify ownership of that email by OTP before submitting.
Admin approves/rejects from the admin dashboard.
On approval a new ASU-AGR researcher ID and full portal record are created automatically.

Replace index.html and admin.html in the GitHub repository root.

IMPORTANT: OTP email requires RESEND_API_KEY and PORTAL_FROM_EMAIL to be configured in Supabase Edge Function secrets before registration emails can actually be sent.
