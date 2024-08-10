# Truecharts

This repository contains the Helm charts for the TrueCharts project, it is important to note that the upcoming release of Truenas Scale Electric Eel, K8S and therefore Truecharts have been removed in favour of native docker / docker-compose files.

## How to fix?
### Dataset is busy

Find the process ID that is using the dataset in `/proc/mounts`
```bash
grep "DATASET NAME" | /proc/*/mounts
```

Kill the process using
```
sudo kill "PROCESS ID"
```
