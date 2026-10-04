<img src="https://lateping.com/og.png" width="512" />

# Lateping

Know when a scheduled job doesn't run. Your job calls a URL when it finishes; if the call is late, or the job reports a failure, you get an alert.

[lateping.com](https://lateping.com) · [Guides](https://lateping.com/guides) · [Pricing](https://lateping.com/pricing) · [Sign in](https://app.lateping.com/login)

## What it does

- Period or cron schedules with timezones and a grace period
- `/start` and `/fail` pings for run times and instant failure alerts
- Alerts by email, Slack, Discord or a signed webhook
- Our own downtime never becomes your alert: missed deadlines are pushed back by the gap
- Setup guides for GitHub Actions, Cloudflare Workers, crontab, Vercel Cron, pg_cron, Kubernetes CronJobs, systemd timers and Laravel
- Free for 10 checks, no card

## Repositories

[lateping](https://github.com/lateping/lateping) is where to report bugs, request features and read the security policy. The service's source is private.

[ping](https://github.com/lateping/ping) is our GitHub Action: one step pings a check when a workflow starts, succeeds or fails.

```yaml
- uses: lateping/ping@v1
  if: always()
  with:
    url: ${{ secrets.LATEPING_URL }}
    status: ${{ job.status }}
```

## Get in touch

[support@lateping.com](mailto:support@lateping.com)

---

<sub>© 2026 JTF Labs Pty Ltd</sub>
