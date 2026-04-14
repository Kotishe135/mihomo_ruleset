# mihomo-rulesets
#### This is my own rulesets for Mihomo
It uses some rules from offical Mihomo's geosite and include my own custom rules
## Usage:
#### config.yml:
```
rule-providers:
  Kotishe135-vpn:
    type: http
    url: https://github.com/Kotishe135/mihomo_ruleset/raw/refs/heads/main/rulesets/vpn.yaml
    interval: 300
    proxy: DIRECT
    behavior: classical
    format: yaml
  Kotishe135-proxy:
    type: http
    url: https://github.com/Kotishe135/mihomo_ruleset/raw/refs/heads/main/rulesets/proxy.yaml
    interval: 300
    proxy: DIRECT
    behavior: classical
    format: yaml
  Kotishe135-direct:
    type: http
    url: https://github.com/Kotishe135/mihomo_ruleset/raw/refs/heads/main/rulesets/direct.yaml
    interval: 300
    proxy: DIRECT
    behavior: classical
    format: yaml
  Kotishe135-reject:
    type: http
    url: https://github.com/Kotishe135/mihomo_ruleset/raw/refs/heads/main/rulesets/reject.yaml
    interval: 300
    proxy: DIRECT
    behavior: classical
    format: yaml
rules:
  - RULE-SET,Kotishe135-reject,REJECT
  - RULE-SET,Kotishe135-proxy,PROXY
  - RULE-SET,Kotishe135-vpn,VPN
  - RULE-SET,Kotishe135-direct,DIRECT
```