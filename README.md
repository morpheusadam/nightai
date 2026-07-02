<div align="center">

# 🪄 MagicAI — AI Content & SaaS Platform

### A full-featured Laravel AI SaaS that turns prompts into text, images, chat, code, voice and video — with multi-provider AI engines, subscriptions and payments built in.

<p>
  <img src="https://img.shields.io/github/license/morpheusadam/NightAI?style=for-the-badge&color=4c1" alt="License" />
  <img src="https://img.shields.io/github/stars/morpheusadam/NightAI?style=for-the-badge&color=ffca28" alt="Stars" />
  <img src="https://img.shields.io/github/forks/morpheusadam/NightAI?style=for-the-badge&color=42a5f5" alt="Forks" />
  <img src="https://img.shields.io/github/last-commit/morpheusadam/NightAI?style=for-the-badge&color=8e44ad" alt="Last commit" />
  <img src="https://img.shields.io/github/repo-size/morpheusadam/NightAI?style=for-the-badge&color=e67e22" alt="Repo size" />
</p>

<p>
  <img src="https://img.shields.io/badge/PHP-8.2%2B-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP" />
  <img src="https://img.shields.io/badge/Laravel-10-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel" />
  <img src="https://img.shields.io/badge/Livewire-3-FB70A9?style=for-the-badge&logo=livewire&logoColor=white" alt="Livewire" />
  <img src="https://img.shields.io/badge/Alpine.js-3-8BC0D0?style=for-the-badge&logo=alpinedotjs&logoColor=black" alt="Alpine.js" />
  <img src="https://img.shields.io/badge/Tailwind%20CSS-3-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS" />
  <img src="https://img.shields.io/badge/MySQL-Database-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL" />
  <img src="https://img.shields.io/badge/Vite-Build-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite" />
</p>

<p>
  <img src="https://skillicons.dev/icons?i=php,laravel,mysql,tailwind,js,vite" alt="Tech stack" />
</p>

</div>

---

## 📖 Overview

**MagicAI** is a complete **AI content-generation SaaS platform** built on **Laravel 10 / PHP 8.2**. It lets you spin up your own "AI as a service" product where users write prompts and get back articles, marketing copy, chat answers, source code, images, voiceovers and video — all behind a subscription and billing layer you control.

Under the hood, MagicAI uses a pluggable **engine-driver architecture** (`app/Domains/Engine`) that connects to many AI providers, so you are not locked into a single vendor: **OpenAI, Anthropic, Google Gemini, DeepSeek, xAI, OpenRouter, Together, ElevenLabs, Stable Diffusion, ClipDrop, Freepik, Synthesia, HeyGen** and more are all wired in as drivers. The frontend is a modern **Livewire + Alpine.js + Tailwind CSS** stack (bundled with Vite), including a TipTap-based rich editor, while the backend ships with multi-language support, role/permission management, an admin panel, and a long list of payment gateways.

It is built for **founders, agencies, and indie hackers** who want to launch a branded AI writing/image/chat product quickly on a battle-tested Laravel codebase.

> 🔎 **Keywords:** MagicAI, Laravel AI SaaS, AI content generator, OpenAI Laravel, AI writing platform, AI image generator, AI chat bot, text to speech, AI SaaS starter, subscription billing, multi-provider AI engine.

> ⚠️ **Note:** GitHub auto-detects this repository as JavaScript because of the bundled frontend assets, but MagicAI is primarily a **PHP / Laravel** application.

---

## ✨ Features

- 📝 **AI text & content** — generate articles, marketing copy, emails and more from templates and prompts.
- 💬 **AI chat** — conversational assistants powered by your chosen LLM provider.
- 🖼️ **AI images** — text-to-image generation via providers like Stable Diffusion, ClipDrop and Freepik.
- 🎙️ **AI voice & speech** — text-to-speech and audio via ElevenLabs / Speechify and Google TTS.
- 🎬 **AI video** — video generation through drivers such as Synthesia, HeyGen, Creatify and Vizard.
- 🔌 **Multi-provider engines** — OpenAI, Anthropic, Gemini, DeepSeek, xAI, OpenRouter, Together and many more via a unified driver layer.
- 💳 **Payments & subscriptions** — Stripe (Cashier), PayPal, Paddle, Razorpay, Iyzico, Cryptomus, CoinGate, YooKassa and others.
- 👥 **Users, roles & permissions** — built on `spatie/laravel-permission`, with an admin dashboard.
- 🌍 **Multi-language** — localization via `mcamara/laravel-localization`.
- 🧩 **Extensible** — Artisan commands to scaffold extension controllers, models and migrations.
- 🔐 **2FA & social login** — Google2FA plus Socialite (including Apple sign-in).
- ⚡ **Modern frontend** — Livewire 3, Alpine.js, Tailwind CSS and a TipTap editor, bundled with Vite.
- 📡 **Realtime & broadcasting** — Pusher / Ably / Laravel Echo support and Laravel Octane.

---

## 🛠️ Tech Stack

| Layer | Technology |
| --- | --- |
| Language | PHP 8.2+ |
| Framework | Laravel 10 |
| Server runtime | Laravel Octane (optional) |
| UI / Reactivity | Livewire 3, Alpine.js |
| Styling | Tailwind CSS 3 |
| Editor | TipTap |
| Build | Vite + Gulp |
| Database | MySQL |
| Realtime | Pusher / Ably / Laravel Echo |
| Auth | Sanctum, Passport, Socialite, Google2FA |
| Testing | Pest / PHPUnit |

---

## 🚀 Getting Started

### Prerequisites

- **PHP 8.2+** with `ext-curl` and `ext-zip`
- **Composer**
- **Node.js + npm**
- **MySQL** database

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/morpheusadam/NightAI.git
cd nightai

# 2. Install PHP & JS dependencies
composer install
npm install

# 3. Configure environment
cp .env.example .env
php artisan key:generate
# then edit .env: DB_*, MAIL_*, and your AI provider / payment keys

# 4. Run migrations
php artisan migrate

# 5. Build front-end assets
npm run build      # or: npm run dev

# 6. Serve the app
php artisan serve
```

> 💡 Set `APP_NAME`, your database credentials, and the API keys for the AI engines and payment gateways you intend to use in `.env`.

---

## ⚙️ Configuration

- **AI engines** live in `app/Domains/Engine/Drivers/*` and are configured via provider config files (`config/openai.php`, `config/gemini.php`, `config/deepseek.php`, …) and matching `.env` keys.
- **Payments** are configured under `config/` (e.g. `config/cashier.php`, `config/paypal.php`, `config/2checkout.php`) plus their `.env` credentials.
- **Localization** is handled by `mcamara/laravel-localization` (`config/laravellocalization.php`).
- **Realtime** broadcasting uses the Pusher/Ably variables in `.env`.

---

## 🗂️ Project Structure

```text
nightai/ (MagicAI)
├── app/
│   ├── Actions/                 # single-purpose action classes
│   ├── Console/Commands/        # Artisan commands (cron, cleanup, extensions)
│   ├── Domains/Engine/          # AI engine drivers + service layer
│   └── Services/                # integrations & helpers
├── config/                      # framework + provider/payment config
├── database/                    # migrations, factories, seeders
├── resources/                   # Blade views, JS, CSS
├── routes/                      # web/api/console routes
├── packages/magicai/            # bundled MagicAI packages (updater, healthy)
├── composer.json                # PHP dependencies (Laravel 10)
├── package.json                 # front-end build (Vite, Tailwind, TipTap)
└── .env.example
```

---

## 🤝 Contributing

Contributions are welcome! Open an [issue](https://github.com/morpheusadam/NightAI/issues) or submit a pull request. Please run the test and lint suites before submitting:

```bash
composer test      # Pest test suite
composer lint      # Laravel Pint code style
```

## 📜 License

Built on the **Laravel framework**, which is open-sourced under the **MIT License**. See [`LICENSE`](LICENSE) for the repository's license terms.

---

<div align="center">

### 👤 Author — Morpheus Adam

Web developer & cheerful hacker · PHP · Laravel · Go

<p>
  <a href="https://github.com/morpheusadam"><img src="https://img.shields.io/badge/GitHub-morpheusadam-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
  <a href="https://sam.zeonic.me"><img src="https://img.shields.io/badge/Website-sam.zeonic.me-4c1?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Website" /></a>
  <a href="mailto:morpheusadam95@gmail.com"><img src="https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

⭐ **If MagicAI helps you launch your AI product, consider giving it a star!** ⭐

</div>


---

## ⭐ Star History

<a href="https://star-history.com/#morpheusadam/NightAI&Date">
  <img src="https://api.star-history.com/svg?repos=morpheusadam/NightAI&type=Date" alt="nightai — Star History Chart" width="70%" />
</a>

<div align="center">

### If this project helps you, please give it a ⭐

A star helps other developers discover **nightai** and supports continued development.

</div>
