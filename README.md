# 中電喵 SCAICT uwu
A can living in SCAICT Discord Group

[![Sync issues to Notion](https://github.com/SCAICT/SCAICT-uwu/actions/workflows/notion.yml/badge.svg?event=issues)](https://github.com/SCAICT/SCAICT-uwu/actions/workflows/notion.yml)

![](thumbnail.png)

> This project is still in beta. If you have any problem, it works on my machine.

## How to run?

1. Clone this repo
2. Create python environment in 3.11
2. Install independance.

```bash
pip install flask py-cord mysql-connector-python requests
```

1. Config channels in DataBase/server.config.json
2. Run SQL Server
3.   Config SQL Server in BreadcrumbsSCAICT-uwu/cog/core/sqlAcc.py
1.   `flask run`
2.   `python main.py`

## Files

* main.py: Discord Bot
* app.py: Flask Web App
* generate-secrets.py: Generate Secret Key for app.py. Run and save it in token.json
* Database MySQL:使用外部伺服器，相關設定在cog/core/secret.py
* token.json

```json
{
    "discord_token":"",
    "secret_key":"",
    "discord_client_id":"",
    "discord_client_secret":"",
    "discord_redirect_uri":"http://127.0.0.1:5000/callback",
    "github_client_id":"",
    "github_client_secret":"",
    "github_redirect_uri":"http://127.0.0.1:5000/github/callback",
    "github_discord_redirect_uri": "http://127.0.0.1:5000/github/discord-callback"
    
}
```
* database/slot.json

Set the possibility for slot machine.

```
 {
    "element": [percentage,reward]
 }
 ```


## credits

Made by SCAICT

<a href="https://www.flaticon.com/free-icons/slot-machine" title="slot machine icons">Slot machine icons created by Freepik - Flaticon</a>
