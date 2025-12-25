# Domain & Subscription Log

## Current Status (as of Dec 24, 2025)

### Domain: officefullofmonkeys.com
- **Registrar**: Wix.com
- **Last Payment**: Jan 27, 2024
- **Expires**: Dec 28, 2026
- **Auto-Renew**: OFF ✅
- **Cost**: ~$30/year ($60 for 2 years)
- **Action Needed**: Consider transferring to cheaper registrar before expiration

### Premium Plan: Light
- **Provider**: Wix.com
- **Last Payment**: Jan 13, 2025
- **Expires**: Jan 8, 2026
- **Auto-Renew**: OFF ✅
- **Status**: Can be cancelled - not needed if building from scratch
- **Action Needed**: Cancel before Jan 8, 2026 or just let it expire

---

## Migration Plan

### Phase 1: Setup (Now - Jan 2026)
- [x] Create static landing page locally
- [ ] Push to GitHub repository
- [ ] Test on GitHub Pages with temporary URL
- [ ] Add GitHub Sparks app links
- [ ] Add Substack link

### Phase 2: Hosting Migration (Jan - Dec 2026)
- [ ] Deploy to GitHub Pages or Cloudflare Pages (FREE)
- [ ] Cancel Wix Premium Light plan (saves ~$10-20/month)
- [ ] Keep domain at Wix until Dec 2026 expiration

### Phase 3: Domain Transfer (Before Dec 28, 2026)
- [ ] Choose new registrar:
  - Cloudflare Registrar (~$10/year)
  - Porkbun (~$10/year)
  - Namecheap (~$12/year)
- [ ] Unlock domain at Wix (90 days before expiration)
- [ ] Get authorization code from Wix
- [ ] Initiate transfer to new registrar
- [ ] Update DNS to point to GitHub Pages/Cloudflare Pages

---

## Cost Comparison

| Service | Current (Wix) | Proposed | Savings/Year |
|---------|---------------|----------|--------------|
| Domain | $30/year | $10/year | **$20** |
| Hosting | ~$96/year (Light plan) | $0 (GitHub Pages) | **$96** |
| **TOTAL** | **~$126/year** | **$10/year** | **$116/year** 🎉 |

---

## Important Dates

- **Jan 8, 2026** - Wix Premium Light expires (let it expire, don't renew)
- **Sep 28, 2026** - Start domain transfer process (90 days before expiration)
- **Dec 28, 2026** - Domain expires at Wix (must transfer before this)

---

## Notes

- Domain auto-renew is already OFF ✅
- Premium plan auto-renew is already OFF ✅
- No rush to cancel Premium Light - it's paid until Jan 2026
- Domain is safe until Dec 2026
- Can migrate hosting anytime (site is ready now)

---

## GitHub Pages Setup Log

### Dec 24, 2025 - Initial DNS Configuration
- **Status**: DNS check unsuccessful (InvalidCNAMEError)
- **Issue**: Custom subdomain `www.officefullofmonkeys.com` not properly configured
- **Required**: CNAME record pointing to `frasod.github.io`
- **Current DNS**: CNAME record created at Wix pointing `www` → `frasod.github.io`
- **TLS Certificate**: Provisioning in progress (up to 15 minutes)
- **Action**: Wait for DNS propagation (5-60 minutes), then check again

### DNS Configuration at Wix
```
Type: CNAME
Host: www.officefullofmonkeys.com
Value: frasod.github.io
TTL: 1 Hour
```

### Troubleshooting
- DNS changes can take up to 48 hours to propagate globally
- GitHub needs to verify CNAME before issuing HTTPS certificate
- Use `dig www.officefullofmonkeys.com` to check DNS propagation
- Once DNS check passes, enable "Enforce HTTPS" in GitHub Pages settings
