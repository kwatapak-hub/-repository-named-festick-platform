# Deploy using an Android phone
1. Download and unzip the starter project.
2. In Chrome, create a private GitHub repository named `festick-platform`. Upload the files/folders so `app`, `supabase`, and `package.json` are at repository root. Use Chrome's desktop-site option if needed.
3. Create a Supabase project. Open SQL Editor, paste `supabase/schema.sql`, and run it. Before connecting a public app, add and test strict Row Level Security policies for customers, organisers and admins.
4. Sign in to Vercel with GitHub. Add New → Project, import the repository, then deploy.
5. Add environment variables from `.env.example` in Vercel project settings. Keep `PAYSTACK_SECRET_KEY` server-side only.
6. Create/verify a Paystack South Africa account. Start with test keys and configure the webhook to `https://YOUR-VERCEL-URL/api/paystack/webhook`.
7. The payment initialization endpoint is deliberately disabled. Implement trusted order creation, server-calculated pricing, inventory locking, verified webhooks, unique QR tickets, single-use scan validation, and email delivery before any live payments.
8. Before launch, test failures, duplicate webhooks, sold-out events, reused/invalid QR codes and refunds. Publish terms, privacy and refund policies and review POPIA requirements.
