# fly_gitea

Template for deploying [Gitea](https://gitea.io/en-us/) on [fly.io](https://fly.io).

## Deploy

SQLite is used by default, but you can use a postgres database by changing environment variables in `fly.toml` and provisioning a postgres database.

`flyctl launch --name fly-gitea --no-deploy --region yyz`

`flyctl volumes create fly_gitea_data --size 1 --region yyz --app fly-gitea`

`flyctl deploy`
