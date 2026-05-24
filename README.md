# TK FUCKER V2

Multi-tool for TikTok views, shares, and Twitch followers.

## Features

| Option | Tool | Description |
|--------|------|-------------|
| 1 | TikTok Viewer | Sends video views (~150/s) |
| 2 | TikTok Sharer | Sends shares (Ctrl+C to stop) |
| 3 | Twitch Follow Bot | Sends follows using OAuth tokens |

## Usage

```bash
./tk-fucker
```

Select from the menu and follow the prompts.

### TikTok Viewer
- Enter a video URL or numeric video ID
- Specify the number of views
- Progress is displayed in real-time

### TikTok Sharer  
- Enter a video URL or numeric video ID
- Runs until you press Ctrl+C
- No target amount — unlimited sharing

### Twitch Follow
- Requires a proxy (`user:pass@host:port`)
- Requires `accounts.txt` with OAuth tokens (one per line)
- 60K+ free, non-expiring tokens included

## Files

| File | Purpose |
|------|---------|
| `main.go` | Source code |
| `accounts.txt` | Twitch OAuth tokens (60K+, never expire) |

## Build

```bash
go build -o tk-fucker .
```

## Notes

- No accounts or proxies needed for TikTok Viewer/Sharer
- Device fingerprints are auto-generated and rotated per request
- Twitch follows require both a proxy and token file
