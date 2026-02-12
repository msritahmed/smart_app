# smart_app

Smart Bookmark App
Tech Stack

Next.js App Router

Supabase (Auth, DB, Realtime)

Tailwind CSS

Vercel Deployment

Features

Google Login Only

Private Bookmarks

Real-time Sync

Add + Delete Bookmarks

Multi-tab Sync

Problems Faced & Solutions
❌ OAuth Redirect Errors

Problem: Login stuck after Google login
Solution: Added correct redirect URL in:

Google Console

Supabase Auth settings

❌ Realtime Not Working on Deploy

Problem: Worked locally but not on Vercel
Solution:
Moved realtime subscription to client component.

(Realtime websockets must run on client in serverless hosting)

❌ Users Seeing Others Data

Problem: Security risk
Solution:
Enabled RLS policies using auth.uid().

❌ Session Expiry Issues

Problem: Users logged out unexpectedly
Solution:
Updated Supabase keys and rotated JWT keys.


<img width="1434" height="927" alt="Screenshot 2026-02-12 191032" src="https://github.com/user-attachments/assets/faa4c3a8-8372-4aa0-a674-5963404500b8" />

