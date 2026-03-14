# Maintenance Guide: Saranga AI Astro Landing Page

This document provides essential information for maintaining the Saranga AI Astro landing page.

## Contact Form (Web3Forms)
The contact form uses [Web3Forms](https://web3forms.com/) for email delivery.
- **Access Key**: `2b84e4da-4a82-4e13-954b-06c9f76eb527`
- **Destination Email**: `sarangapanchangam@gmail.com`
- **Dashboard**: You can manage submissions and settings at [web3forms.com](https://web3forms.com/).

## Ad Monetization (app-ads.txt)
To ensure uninterrupted ad revenue, the `app-ads.txt` file is required by various ad networks.
- **Locations**:
  - Root: `/app-ads.txt`
  - Public folder: `/public/app-ads.txt`
- **Current Content**:
  ```text
  google.com, pub-2812900831697343, DIRECT, f08c47fec0942fa0
  facebook.com, 675792898941096, DIRECT, c3e20eee3f780d68
  inmobi.com, b1e81b61bdb94928afc6df97608bfaaa, DIRECT, 83e75a7ae333ca9d
  ```

## Deployment
The site is hosted on **Cloudflare Pages** and integrated with the GitHub repository:
- **Repository**: `https://github.com/nd-balaji/AiAstroWeb.git`
- **Automation**: Any push to the `main` branch triggers an automatic deployment to [aipanchangam.pages.dev](https://aipanchangam.pages.dev/).

## Visual & Interaction
- **Style**: 'Premium Indigo' Dark Mode (Tailwind CSS).
- **Localization**: Supports English (EN) and Tamil (TA) toggles.
- **Panchangam**: Real-time Tithi and Nakshatra calculations based on the user's local clock.
