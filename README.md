# fleamspeak
Run a teamspeak3 server on fly.io!

## How to run

```bash
$ fly apps create ts3-server
$ fly volumes create ts3_data --region fra --size 1 --app ts3-server
$ fly deploy --remote-only --config fly.toml
```
