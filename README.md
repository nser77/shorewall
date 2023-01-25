# SHOREWALL

SHOREWALL repository for a server installation with HA and WIREGUARD support.

The repo was tested with ``` Shorewall 5.0, 5.1 and 5.2 ```.

Remeber to eneble Shorewall daemon:

```
if [ "$(systemctl is-enabled shorewall)" == "disabled" ]; then systemctl enable shorewall; fi
```

## Loopback for DNS
SHOREWALL's start and stop scripts create ```dummy``` interface that could be used as global DNS for all peers.

## WIREGUARD
If you want to use this configuration with WIREGUARD, setup your VPN-Server then adapt the file ```params``` as you need.

### IPv4 Kernel Forward:
You may want to enable Kernel forward.

```
echo "net.ipv4.ip_forward = 1" > /etc/sysctl.d/11-network-ipv4-ip_forward.conf && sysctl --system
```
