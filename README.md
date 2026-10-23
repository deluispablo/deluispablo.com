# deluispablo.com

Portfolio of Pablo de Luis, live at [deluispablo.com](https://deluispablo.com).

| Path | Project |
|---|---|
| [`/healthtracker/`](https://deluispablo.com/healthtracker/) | [Health Tracker](https://github.com/deluispablo/health-tracker): a Pixel Watch app, a dashboard and an analysis server for your own health data |

## How it works

- `public/` is the whole site. A Cloudflare Worker serves it as static assets (`wrangler.jsonc`) on `deluispablo.com` and `www.deluispablo.com`, and every push to `main` deploys it.
- `public/_redirects` sends the root to `/healthtracker/` until the portfolio has its own home page.
- Each project keeps its page in its own repository. `public/healthtracker/index.html` is a copy of `landing/index.html` from health-tracker, refreshed every day by the **Sync Health Tracker landing** workflow, or on demand from the Actions tab.

## License

[MIT](LICENSE)
