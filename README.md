# farooks.com

GitHub Pages site for **farooks.com** — home of the Farooks.

## Repo Structure

```
main/
├── index.html   # Single-page dark theme, links to family subdomains
├── CNAME        # Custom domain: farooks.com
├── .gitignore
└── README.md
```

## Enable GitHub Pages

1. Go to **Settings → Pages** in this repo.
2. Source: branch `main`, folder `/ (root)` → **Save**.
3. Custom domain: `farooks.com` → **Save**.
4. Check **Enforce HTTPS** once the DNS certificate provisions.

## Namecheap DNS — Point farooks.com to GitHub Pages

In your Namecheap dashboard for **farooks.com**, go to **Advanced DNS** and add/update:

### Apex domain (farooks.com) — A records

| Type | Host | Value          | TTL       |
|------|------|----------------|-----------|
| A    | @    | 185.199.108.153 | Automatic |
| A    | @    | 185.199.109.153 | Automatic |
| A    | @    | 185.199.110.153 | Automatic |
| A    | @    | 185.199.111.153 | Automatic |

### www redirect (optional)

| Type  | Host | Value                | TTL       |
|-------|------|----------------------|-----------|
| CNAME | www  | meshameer.github.io. | Automatic |

> GitHub Pages apex domain requires A records (not a CNAME).
> DNS propagation can take a few minutes to 48 hours.
