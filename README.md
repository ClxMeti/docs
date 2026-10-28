# دثره فروش

- صفحهٔ اصلی: `index.html`
- استایل مشترک: `styles.css`
- رفتارهای تعاملی: `app.js`
- برای صفحه‌های بعدی از `pages/*.html` و لینک‌های نسبی استفاده کنید.
- فایل‌ها در پیش‌نمایش زنده مستقیماً اجرا می‌شوند؛ وابستگی به build یا npm اضافه نکنید.

## Go API

- Source: `backend/main.go`; module: `backend/go.mod`.
- Endpoints in the project preview use `/api/...` and run in an isolated container.
- Keep the server on `127.0.0.1:8080` and use Go standard-library packages.
- Frontend requests should use `window.MONETIZEAI_API_BASE` in the platform preview, with `/api/` as the self-hosting fallback.
- `backend/monetize_runtime.go` provides persistent JSON storage, secure password hashing, uploads and allowlisted external API requests.
