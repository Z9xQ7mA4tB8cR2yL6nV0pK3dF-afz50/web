# web

my web project - VNC Browser with Cloudflare Tunnel

## Workflow: web-tunnel

GitHub Actions e `web-tunnel` workflow run korle:
1. Ubuntu VM e Xvfb + VNC Server setup hobe
2. Full Chrome browser chalbe (headless na)
3. noVNC Web interface available
4. Cloudflare tunnel create hobe
5. Tunnel URL visit korle full browser pabe
6. Workflow running thakbe (manual cancel na korle)

**Run:**
```bash
gh workflow run web-tunnel
```

**Tunnel URL logs e pabe, then:**
1. URL open korle noVNC interface asbe
2. "Connect" click korlei browser pabe
3. Full interaction - tab open/close, click, type, search - sob kaj korbe
