# NyroxHub email backend

This service sends real emails through Gmail SMTP. Never commit `.env` or your App Password.

## Environment

Copy `.env.example` to `.env` and set:

- `SMTP_HOST=smtp.gmail.com`
- `SMTP_PORT=465`
- `SMTP_SECURE=true`
- `SMTP_USER=smtp.nypay@gmail.com`
- `SMTP_PASSWORD=<Google App Password>`
- `PUBLIC_URL=<public backend URL>`

Install and run:

```bash
npm install
npm start
```

Endpoints:

- `POST /api/register` — creates a normal `user` account and sends a welcome email.
- `POST /api/forgot-password` — sends a 15-minute password reset link.
- `POST /api/reset-password` — consumes a reset token.
- `POST /api/order-email` — sends an order notification without claiming payment success.

For production, replace the in-memory user/reset storage with a real database and hash passwords with a password-hashing library. Do not use the example storage as a production authentication database.
