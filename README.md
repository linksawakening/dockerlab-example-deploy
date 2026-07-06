# dockerlab-example-deploy

Example DockerLab deployment with SearXNG.

## Bootstrap on production-host

Run as root:

```bash
curl -fsSL https://raw.githubusercontent.com/linksawakening/dockerlab-deploy/main/scripts/install.sh | \
  bash -s -- \
    --deployment-repo https://github.com/linksawakening/dockerlab-example-deploy.git \
    --deployment-dir /opt/dockerlab-example-deploy \
    --user dockerlab-deploy \
    --interval 5min
```

Then create `/opt/dockerlab-example-deploy/.env` from `.env.example`.
