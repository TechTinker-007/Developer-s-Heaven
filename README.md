<div align="center">

# 🏗️ Developer's Heaven

### Material logistics tracking for real estate & construction projects — built for people who are tired of spreadsheets and WhatsApp chaos.

[![Made with React](https://img.shields.io/badge/Frontend-React%20%2B%20TypeScript-61DAFB?style=for-the-badge&logo=react&logoColor=white)](https://react.dev)
[![Powered by Supabase](https://img.shields.io/badge/Backend-Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)](https://supabase.com)
[![Styled with Tailwind](https://img.shields.io/badge/Styling-Tailwind%20CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com)
[![Deployed on Vercel](https://img.shields.io/badge/Deployed-Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://vercel.com)
[![License](https://img.shields.io/badge/License-All%20Rights%20Reserved-red?style=for-the-badge)](./LICENSE)

**[✨ Live Demo](#) · [📖 Features](./FEATURES.md) · [🔍 Detailed Docs](./FEATURES_DETAILED.md) · [🗺️ Roadmap](./CHANGELOG.md)**

</div>

---

## 🚀 Why Developer's Heaven?

> Managing construction material logistics across spreadsheets and chat threads is messy, error-prone, and impossible to audit. **Developer's Heaven centralizes it** — every delivery, every unit used, every rupee spent, tracked per project, visualized in real time.

<table>
<tr>
<td width="50%" valign="top">

### 🎯 Built For
- Site engineers
- Contractors
- Project managers
- Anyone drowning in material Excel sheets

</td>
<td width="50%" valign="top">

### 💡 Built With
- AI-assisted development (Claude), used honestly and disclosed
- A prompt-driven, additive-only build philosophy
- Zero terminal deployment — 100% GUI workflow

</td>
</tr>
</table>

---

## ✨ Feature Highlights

| 🧱 Module | What it does |
|---|---|
| **📦 Material Log** | Log every delivery & usage entry — quantity, unit, price, supplier |
| **📊 Stock** | Live stock levels, auto-calculated from deliveries − usage |
| **🏢 Suppliers** | Compare pricing, spend, and reliability across suppliers |
| **💰 Total Summary** | Budget vs. spend, with instant over-budget flags |
| **📈 Visual Analytics** | 6+ charts — spend trends, cost share, delivered vs. used, and more |
| **🔔 Alerts** | Budget threshold & delivery-date notifications *(in progress)* |

> 📖 **Want the full breakdown?** See [FEATURES.md](./FEATURES.md) for the quick list or [FEATURES_DETAILED.md](./FEATURES_DETAILED.md) for field-by-field detail.

---

## 🖼️ Screenshots

<div align="center">

*Add your screenshots here — Material Log, Suppliers, Visual Analytics dashboards look great as a 2x2 grid.*

</div>

---

## 🛠️ Tech Stack

<div align="center">

| Layer | Technology |
|:---:|:---:|
| **Frontend** | Vite ⚡ + React ⚛️ + TypeScript |
| **Styling** | Tailwind CSS 🎨 |
| **Backend** | Supabase (Postgres + Auth + RLS) 🔐 |
| **Deployment** | GitHub → Vercel 🚀 |

</div>

---

## 🚦 Getting Started

### ✅ Prerequisites
- Node.js 18+
- A Supabase project (free tier works fine)

### ⚙️ Setup

```bash
git clone https://github.com/<your-username>/Developer-s-Heaven.git
cd Developer-s-Heaven
npm install
```

Create a `.env` file in the project root (see [`.env.example`](./.env.example)):

```env
VITE_SUPABASE_URL=your_supabase_project_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
```

> ⚠️ **Security note:** Only the **anon/public** key belongs on the client. Row Level Security (RLS) policies enforce all data access — see [Security](#-security) below.

Run locally:

```bash
npm run dev
```

---

## 📁 Project Structure

```
Developer-s-Heaven/
├── src/
│   ├── components/       # UI components (forms, tables, charts)
│   ├── pages/             # Route-level pages (Material Log, Stock, Suppliers, etc.)
│   ├── lib/                # Supabase client, helpers
│   ├── types/              # TypeScript types
│   └── App.tsx
├── public/
├── .env.example
└── README.md
```

---

## 🔒 Security

- ✅ Row Level Security (RLS) enforced on all Supabase tables, scoped per authenticated user/project
- ✅ No secrets or service-role keys exposed client-side
- ✅ Input validation on all form fields
- ✅ Session-based auth with proper logout/session clearing

---

## 🗺️ Roadmap

> 🔜 Custom unit creation · Supplier-attributed price ranges · Real-time budget alerts · Delivery-date notifications · Performance optimization pass

See [CHANGELOG.md](./CHANGELOG.md) for full version history and what's planned next.

---

## 📄 License

**All Rights Reserved.** This project is proprietary — see [LICENSE](./LICENSE) for details.

---

## 🤝 Contributing

This is currently a solo-maintained project, but bug reports and suggestions are always welcome. See [CONTRIBUTING.md](./CONTRIBUTING.md) to get started.

---

<div align="center">

**Built with 🧠 + ☕ by [Jahar Singh](https://github.com/<your-username>)**

If this project helped you think about your own site logistics — a ⭐ goes a long way.

</div>
