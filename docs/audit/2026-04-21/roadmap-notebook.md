# Wallestars Ultimate Workspace — Condensed Knowledge Base

## Vision
Unified ecosystem combining card management (Wallester + Revolut), SMS/OTP infrastructure, Android cloud automation (DuoPlus + NodeMaven), cloud browsers (Browserbase), and an AI voice agent "Молти 🦞" (Claude + ElevenLabs + Whisper) — operated from a self-hosted n8n + Supabase + Cloudflare stack on Hostinger VPS `srv1201204`.

## Six Phases
1. **Foundation** — audit, secrets, repos, VPS hardening, backups, SSL, logging, uptime, docs.
2. **Core APIs** — Wallester cards + Revolut Business + SMS pool.
3. **Automation** — DuoPlus devices + NodeMaven proxies + Browserbase sessions + task queue.
4. **AI Layer** — ElevenLabs TTS + Whisper STT + Claude brain + memory + intent routing + multi-channel bot.
5. **Observability** — Grafana + anomaly detection + RLS audit + rate limits + runbooks + pentests.
6. **Scale** — auto-scale + cost dashboard + legacy migration + Prime Time Launch.

## Security posture
- SSH keys only on VPS (no password)
- fail2ban + UFW
- Supabase RLS on every table
- Secrets in vault (Doppler or Supabase Vault)
- Daily backups off-site
- Alerting to Slack + Telegram

## Bot
"Молти 🦞" classifies intent with Claude → triggers n8n workflows → speaks back via ElevenLabs. Available via Telegram, Discord, and web dashboard.

## Known open issues
- `ssh srv1201204` fails with `Permission denied (publickey)` — add key to VPS.
- Docker daemon off on Mac.
- GitHub PAT lacks write scope on Wallestars repos — rotate.
