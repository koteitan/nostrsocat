# nostrsocat
websocat wrapper for nostr with bash completion

## Requrements
- websocat
- bash

## Install
```bash
sudo apt install websocat
git clone git@github.com:koteitan/nostrsocat
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
nostrsocat wss://yabu.me authors [\"$mypub\"] kinds [0]
```

## Tips
if you have jq, you can use it like this
```bash
nostrsocat wss://yabu.me authors [\"$mypub\"] kinds [0] | jq -r
```

If you want to use the your public key multiple times, you can export it like this
```bash
export mypub=4c5d5379a066339c88f6e101e3edb1fbaee4ede3eea35ffc6f1c664b3a4383ee
```

