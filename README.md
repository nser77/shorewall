# shorewall

Shorewall repository for a server installation.

The repo was tested with ``` Shorewall 5.2.3.4 ```.

Remeber to eneble Shorewall daemon:

```
root@jammy:/home/user# if [ "$(systemctl is-enabled shorewall)" == "disabled" ]; then systemctl enable shorewall; fi
```
