# Dummy-Systemd-Service-DevOps-roadmap
Dummy Systemd Service project for DevOps roadmap
https://roadmap.sh/projects/dummy-systemd-service

## Move dummy.service to /etc/system/dummy.service
```
sudo cp dummy.service /etc/systemd/system/dummy.service
```

## Move dummy.sh to /usr/local/bin/dummy.sh
```
sudo cp dummy.sh /usr/local/bin/dummy.sh
sudo chmod +x /usr/local/bin/dummy.sh
```

## Reload and start service
```
sudo systemctl daemon-reload
sudo systemctl start dummy
sudo systemctl enable dummy
sudo systemctl status dummy
```

## Check logs
```
sudo journalctl -u dummy -f
```