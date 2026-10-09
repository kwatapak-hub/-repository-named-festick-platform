# Festick platform starter
Phone-friendly Next.js starter for a South African event ticketing platform.

Includes a responsive landing page, Supabase schema, Paystack webhook signature verification, and Android deployment instructions.

Important: this is a starter, not production-ready. The checkout endpoint intentionally refuses payments until server-side order lookup and price calculation are implemented. Before launch, finish and test RLS policies, payment verification, ticket/QR issuance, single-use scanning, email delivery, refunds, POPIA/privacy notices and backups. Never expose secret keys in browser code.
