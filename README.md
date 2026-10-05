# SilverDrop PNW — sample site

**Live (temporary):** https://phillanneanderson-ai.github.io/

**Custom domain (pending DNS):** https://silverdroppnw.com/

Hosted on **GitHub Pages** (free) from this repo (`phillanneanderson-ai.github.io`).

## Point silverdroppnw.com here (Porkbun)

Domain is still on Porkbun’s Link-in-Bio (`silverdroppnw-com.l.ink`). To serve this site on the apex domain:

1. Log in at https://porkbun.com with **phillanneanderson@gmail.com**.
2. **Domain Management** → **silverdroppnw.com** → **DNS**.
3. **Disable / remove** Link-in-Bio, URL forward, or any ALIAS/URL record that sends traffic to `l.ink` or Porkbun’s placeholder.
4. Add these records (leave WHOIS privacy on; do not buy hosting):

| Type | Host | Answer | TTL |
|------|------|--------|-----|
| A | (blank / @) | `185.199.108.153` | 600 |
| A | (blank / @) | `185.199.109.153` | 600 |
| A | (blank / @) | `185.199.110.153` | 600 |
| A | (blank / @) | `185.199.111.153` | 600 |
| AAAA | (blank / @) | `2606:50c0:8000::153` | 600 |
| AAAA | (blank / @) | `2606:50c0:8001::153` | 600 |
| AAAA | (blank / @) | `2606:50c0:8002::153` | 600 |
| AAAA | (blank / @) | `2606:50c0:8003::153` | 600 |
| CNAME | `www` | `phillanneanderson-ai.github.io` | 600 |

5. Tell Grok Bot DNS is updated so a `CNAME` file (`silverdroppnw.com`) can be committed for GitHub Pages + HTTPS on the custom domain.

Optional: create Porkbun API keys at https://porkbun.com/account/api and enable API Access on the domain so DNS can be automated next time.
