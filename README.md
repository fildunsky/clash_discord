Чтобы у вас работал голос в Discord через Super Simple Clash или что вашей душе угодно:

```yaml
rule-providers:

  discord-domain:
    behavior: classical
    type: http
    url: "https://raw.githubusercontent.com/fildunsky/clash_discord/refs/heads/main/discord-domain.yaml"
    interval: 86400
    path: ./ruleset/discord-domain.yaml

  discord-ip:
    behavior: classical
    type: http
    url: "https://raw.githubusercontent.com/fildunsky/clash_discord/refs/heads/main/discord-ip.yaml"
    interval: 86400
    path: ./ruleset/discord-ip.yaml
```

```
rules:
  - RULE-SET,discord-domain,PROXY
  - RULE-SET,discord-ip,PROXY
```
