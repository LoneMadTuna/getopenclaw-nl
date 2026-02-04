# GetOpenClaw.nl Setup Log

## 2026-02-04: GA4 + ZZP Landing Page

### Google Analytics 4 Setup

**Account:** GetOpenClaw (nieuw account)
**Property:** getopenclaw.nl
**Measurement ID:** `G-VQXTMQ3WTF`
**Stream ID:** 13414974907

**Stappen uitgevoerd:**
1. Nieuw GA4 account aangemaakt (bestaand account had geen Editor rechten voor nieuwe properties)
2. Property `getopenclaw.nl` aangemaakt
3. Web data stream geconfigureerd
4. Enhanced measurement ingeschakeld

**Tracking toegevoegd aan:**
- `index.html` (Eva Jinek homepage)
- `bedankt.html` (bedankpagina na form)
- `zzp.html` (nieuwe ZZP landing page)

### ZZP Landing Page (Marieke Persona)

**Bron:** `/business/products/clawdbot-setup-service/landing-pages/marieke-final.html`
**Doel:** `https://getopenclaw.nl/zzp.html`

**Aanpassingen:**
- Branding: Clawdbot → OpenClaw
- Email: info@clawdbot.com → info@getopenclaw.nl
- Jaar: 2025 → 2026
- GA4 tracking toegevoegd

### Deployment

**Methode:** GitHub → Cloudflare Pages (auto-deploy)
**Repo:** https://github.com/LoneMadTuna/getopenclaw-nl
**Commit:** `1b5f117` - "Add GA4 tracking (G-VQXTMQ3WTF) + ZZP landing page"

### Live URLs

| Pagina | URL | Doel |
|--------|-----|------|
| Homepage | https://getopenclaw.nl | Eva Jinek hook |
| ZZP Landing | https://getopenclaw.nl/zzp.html | ZZP'ers/freelancers |
| Bedankt | https://getopenclaw.nl/bedankt.html | Post-form redirect |

---

## Toekomstige Landing Pages

Beschikbaar in `/business/products/clawdbot-setup-service/landing-pages/`:
- v6-ecommerce → `/shop.html`
- v7-coach → `/coach.html`
- v8-developer → `/dev.html`
- v9-accountant → `/accountant.html`

Proces om toe te voegen:
1. Kopieer naar `/projects/getopenclaw/`
2. Voeg GA4 tracking toe
3. Update branding (Clawdbot → OpenClaw)
4. `git add -A && git commit -m "Add X page" && git push`
