# Easypanel + Docker

Easypanel Schema for using Siim Leaks Basic Discord bot

```yaml
{
  "services": [
    {
      "type": "app",
      "data": {
        "projectName": "discord-bot-siim-leaks-basic",
        "serviceName": "siim-leaks-basic",
        "source": {
          "type": "image",
          "image": "siimleaks/siim-leaks-basic:latest"
        },
        "env": "token = YOUR_BOT_TOKEN\nguild = YOUR_CHANNEL_ID\nleaver_channel_id = YOUR_CHANNEL_LEAVER_CHAT\ncog_ticket_category_id = YOUR_CHANNEL_TICKET_CHAT",
        "proxy": {
          "port": 80,
          "secure": true
        },
        "deploy": {
          "replicas": 1,
          "command": null,
          "zeroDowntime": true
        }
      }
    }
  ]
}
```
