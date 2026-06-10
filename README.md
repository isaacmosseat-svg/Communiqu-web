# Communiqué | Coming Soon

This is the repository for the [Communiqué](https://communique.press) "Coming Soon" page, designed for free hosting on Cloudflare Pages.

## Features

- **Astro & Tailwind CSS:** Built for speed and modern styling.
- **Dark/Light Mode:** Full support with system preference detection and persistence.
- **Responsive Design:** Optimized for mobile, tablet, and desktop.
- **Accessibility (WCAG 2.1):** High contrast, keyboard navigation, and screen reader support.
- **Privacy (GDPR):** Zero cookies, zero trackers, and a clear data policy.
- **Security:** Pre-configured Cloudflare security headers (HSTS, CSP, etc.).

## Setup Instructions

### 1. Cloudflare Account Setup
1. Create a free account at [cloudflare.com](https://www.cloudflare.com/).
2. Add your domain `communique.press`.
3. Follow the instructions to change your **Nameservers** at GoDaddy to the ones provided by Cloudflare.
4. Enable **DNSSEC** in the Cloudflare DNS settings for extra security.

### 2. Connect to Cloudflare Pages
1. Push this repository to your GitHub account.
2. In the Cloudflare Dashboard, go to **Workers & Pages** > **Create application** > **Pages** > **Connect to Git**.
3. Select this repository.
4. Use the following build settings:
   - **Framework preset:** `Astro`
   - **Build command:** `npm run build`
   - **Build output directory:** `dist`
5. Click **Save and Deploy**.

### 3. Configure Custom Domain
1. Once deployed, go to the **Custom domains** tab in your Pages project.
2. Add `communique.press`. Cloudflare will automatically handle the SSL certificate and HTTPS encryption.

### 4. Security Hardening (Best Practice 2026)
- In the Cloudflare dashboard for `communique.press`, ensure the following are enabled:
  - **Always Use HTTPS**: ON
  - **HSTS**: ON
  - **Automatic HTTPS Rewrites**: ON
  - **WAF (Web Application Firewall)**: Enable the default Managed Rulesets (Free tier).

## Local Development

```bash
# Install dependencies
npm install

# Start the development server
npm run dev

# Build for production
npm run build
```

## Compliance Information

- **VZW/ASBL**: Communiqué
- **Address**: Rue Locquenghien 41, 1000 Brussels, Belgium
- **CBE**: 1025.174.291
