# Monitoring container logs using Loki

## Roles
- [x] [Grafana](#Grafana)
- [x] [Loki](#Loki)
- [x] [Promtail](#Promtail)

## Grafana 
> - Add your URL to `GF_SERVER_ROOT_URL` and `GF_RENDERING_CALLBACK_URL` .
> - Add your domain to `GF_SERVER_DOMAIN` .
> - Don't forget to add your domain to `hostname` in traefik labels .

## Promtail

- ### You can use the node-exporter-only ansible to install it on servers you want to monitor.


> [!CAUTION]
> Don't forget to disable the roles you won't need in `setup.yml` file.

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

