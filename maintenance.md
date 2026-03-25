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
- **Current Content**: The file contains Google, Facebook, and InMobi entries, along with an expanded list of 90+ Reseller and Direct entries for various ad networks (Mintegral, Pubmatic, Rubicon, etc.).

## Deployment
The site is hosted on **Cloudflare Pages** and integrated with the GitHub repository:
- **Repository**: `https://github.com/nd-balaji/AiAstroWeb.git`
- **Automation**: Any push to the `main` branch triggers an automatic deployment to [aipanchangam.pages.dev](https://aipanchangam.pages.dev/).

## Visual & Interaction
- **Style**: 'Premium Indigo' Dark Mode (Tailwind CSS).
- **Localization**: Supports English (EN) and Tamil (TA) toggles.
- **Panchangam**: Real-time Tithi and Nakshatra calculations based on the user's local clock.
