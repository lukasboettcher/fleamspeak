# fleamspeak
Run a [Teamspeak 3](https://teamspeak.com/en/) server on [fly.io](https://fly.io)!


## How to run

```bash
$ fly apps create ts3-server
$ fly volumes create ts3_data --region fra --size 1 --app ts3-server
$ fly deploy --remote-only --config fly.toml
```
## How to update
Just redeploy and fly.io will pull the newest image
and seamlessly replace the old container!
```bash
$ fly deploy --remote-only --config fly.toml
```
