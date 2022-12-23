# shorewall

Shorewall repository for a server installation.

The repo was tested with ``` Shorewall 5.0, 5.1 and 5.2 ```.

Remeber to eneble Shorewall daemon:

```
root@jammy:/home/user# if [ "$(systemctl is-enabled shorewall)" == "disabled" ]; then systemctl enable shorewall; fi
```
