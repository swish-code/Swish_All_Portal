# Swish All Portal

Unified Control Center for all Swish Network systems and partner integrations.

A single launchpad with a sci-fi UI that opens 17 internal/external dashboards
(Database, Complaint, Schedule, Technical, Xontel, Ordable, My Fatoorah, Verdi,
Tookan, Talabat, Grubtech, Deliveroo, Respond, Keeta, BillBayt, Do Delivery, Jahez)
with a quantum-tunneling transition animation.

## Local run

```bash
npm start
# http://localhost:3000
```

No dependencies required — pure Node built-ins.

## Deploy on Railway

Configured via `railway.json` (Nixpacks builder, `node server.js`).
Just connect this repo to Railway and it will auto-deploy.

## Tech

- Single-file static HTML/CSS/JS UI (`index.html`)
- Tiny Node.js static file server (`server.js`)
- Inter font from Google Fonts
- Inline SVG icon library, per-card accent colors driven by CSS variables

## Editing the systems list

Open `index.html`, find the `SYSTEMS` array near the top of the inline `<script>`
block. Each entry controls one card: `name`, `icon` (id from the SVG `<defs>`),
`category`, `status`, `desc`, `accent` (hex color), `filled` (1-14 progress
bars), and `url`.
