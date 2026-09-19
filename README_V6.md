ASU Agriculture Research Portal V6 – Unified Email OTP Access

USER FLOW:
1. User enters only official @agr.asu.edu.eg email.
2. System sends a 6-digit one-time code.
3. After OTP verification:
   - If the email exists in Researchers: user is signed in directly to their profile.
   - If the email does not exist: the verified email is locked and a data-completion form appears.
   - If a registration request already exists: the user sees that it is pending.
4. New registration requests require Admin approval.
5. Admin approval creates the researcher and portal records automatically.

UPLOAD:
Replace index.html with this V6 file.
admin.html is included and may replace the current admin.html as well.

IMPORTANT:
Actual OTP delivery requires the Supabase Edge Function secrets:
RESEND_API_KEY
PORTAL_FROM_EMAIL
PORTAL_FROM_NAME (optional)

Until the email provider is configured, keep the current live V5 page if you still need static-code access.
