ASU Agriculture Research Portal – Admin Panel V2 (Excel Export)

IMPORTANT:
- Replace the existing admin.html in the GitHub repository with this new admin.html.
- Do NOT delete index.html.

GitHub Pages admin URL:
https://amrmossad-blip.github.io/-asu-agriculture-research-portal/admin.html

New buttons:
1) تصدير Excel كامل
   - Full live snapshot of the institutional research database.
2) تصدير التغييرات فقط
   - Change log since the previous change-log export.

The exported workbook intentionally excludes:
- access_code_hash
- admin_code_hash
- session token hashes
- Supabase secret/service-role keys

Full workbook sheets:
Summary
Researchers
Portal_Users
Identifiers
Publications
Researcher_Publications
Correction_Requests
New_Publications
Rank_History
Status_History
Audit_Log
Export_History

Backend:
https://xaddbgzrnhaixkqrotkz.supabase.co/functions/v1/admin-export
