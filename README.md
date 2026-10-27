# Traffic Light for Claude Code

Floating macOS traffic lights for Claude Code: one light per live session, so you can see at a glance which sessions
are working and which need you. Spoken summaries, alerts, captions.

This repo holds only release builds. The source is private.

## Install

```bash
curl -fsSL https://github.com/Bixify/traffic-light-releases/releases/latest/download/get.sh | bash
```

Needs macOS 13+ and `jq` (included in macOS 15; otherwise `brew install jq`). Then start a new Claude Code session.

The app updates itself: it checks every hour and installs a new version once no session is busy.
Right-click the light → Settings for options; Settings → Voice → Neural voices adds free offline English and Hebrew voices.

## Remove

Quit the light (right-click → Quit), delete `/Applications/TrafficLight.app`, and remove the `traffic-light` entries
under `hooks` in `~/.claude/settings.json`.
