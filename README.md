# shorewall

Shorewall repository for a server installation wit HA and WIREGUARD support.

The repo was tested with ``` Shorewall 5.0, 5.1 and 5.2 ```.

Remeber to eneble Shorewall daemon:

```
root@jammy:/home/user# if [ "$(systemctl is-enabled shorewall)" == "disabled" ]; then systemctl enable shorewall; fi
```

## wireguard
If you want to use this configuration with WIREGUARD, setup your VPN Server then adapt the file ```params``` as you need.
