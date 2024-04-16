# nostrsocat
websocat and jq wrapper for nostr

## Install
```bash
chmod +x nostrsocat
cp nostrsocat /usr/local/bin
cp nostrsocat_completion /etc/bash_completion.d
source nostrsocat_completion
```
## Usage
```bash
nostrsocat <relay> <key1> <value1> <key2> <value2> ...
```

## Examples
```bash
nostrsocat wss://yabu.me authors [\"$mypub\"] | kinds 0
```

