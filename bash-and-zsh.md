


# Install tools

## Install kubectl
```bash
curl -LO https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl
```


# Archiving history

## History Archiving on zsh

- Used along with clear scrollback, deleted history file, and also history -p

```bash
#!/bin/bash

function saveandquit() {
  cd /Users/<user>/RecordsAndArchives
  export DATE="$(date +%s-%y-%m-%d)"
  echo "$DATE" >> RawData/TerminalHistory/$DATE
  history -n 0 >> RawData/TerminalHistory/$DATE
  history -p
  exit 0
}
```

