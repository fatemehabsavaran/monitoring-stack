# Monitoring tools

## Roles

- [x] grafana-loki-promtail
- [x] grafana-prometheus-node exporter
- [x] uptime kuma

> [!IMPORTANT]  
> Please make sure to comment out any role you won't be needing in `setup.yml` .

## Setup
```
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Run
Add ssh config hostname to `hosts`
```
ansible-playbook setup.yml
```
