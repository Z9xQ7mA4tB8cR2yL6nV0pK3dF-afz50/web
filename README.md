# web

my web project - Selenium Browser with Cloudflare Tunnel

## Workflow: web-tunnel

GitHub Actions e `web-tunnel` workflow run korle:
1. Ubuntu VM e Chrome browser + Selenium setup hobe
2. Headless Chrome browser chalbe
3. Cloudflare tunnel create hobe
4. Sei tunnel browser ke point korbe
5. Workflow choto thakbe (manual cancel na korle)

Run command:
```bash
# Workflow dispatch diye run korar jonnay
gh workflow run web-tunnel
```

View logs:
```bash
gh run watch $(gh run list --workflow web-tunnel --limit 1 --json id --jq '.[0].id')
```
