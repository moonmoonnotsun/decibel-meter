# decibel-meter.app

Landing page for **Decibel Meter: dB Sound Level** (iOS).

## Deploy

Hosted on [GitHub Pages](https://pages.github.com/) with custom domain `decibel-meter.app`.

```bash
git push origin main
```

## GitHub Pages setup

1. Create repo `decibel-meter` on GitHub (public)
2. Push this folder
3. **Settings → Pages →** deploy from `main` branch, root `/`
4. Set custom domain: `decibel-meter.app`
5. Enable **Enforce HTTPS** after DNS check passes

## Cloudflare DNS

For apex domain `decibel-meter.app`:

| Type | Name | Value |
|------|------|-------|
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |
| CNAME | `www` | `moonmoonnotsun.github.io` |

Use DNS only (grey cloud). Set SSL mode to **Full** in Cloudflare.

## Links

- App Store: https://apps.apple.com/us/app/decibel-meter-db-sound-level/id6756241739
- Privacy: https://mpc-app-c2e7a.web.app/decibel-privacy.html
- Terms: https://mpc-app-c2e7a.web.app/decibel-terms.html
