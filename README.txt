AshGuard Front End
===================

Contents
- index.html: responsive AshGuard camera/upload interface.

Deploy with Cloudflare Pages (Direct Upload)
1. In Cloudflare Dashboard, open Workers & Pages.
2. Choose Create application, then Pages (or Create a project > Pages).
3. Choose Direct Upload / Upload your static assets.
4. Upload the ZIP file or the extracted folder containing index.html, following the options shown in your dashboard.
5. Deploy, then open the Pages URL it provides.

This page calls the existing Gemini Worker:
https://ashguard-camera.student-sb-plymouth.workers.dev/

Before public launch:
- The Worker must have GEMINI_API_KEY configured as a secret and be deployed.
- Restrict allowed origins to your published Pages domain and add rate limiting/abuse protection.
- The current “Mark observation as reported” button is a demo badge only. It does not send or store a real report.
- Gemini observations are not a diagnosis.
