# VPN

## Connecting to VPN

```bash
sudo openvpn user.ovpn
```

## Check the connection

```bash
ifconfig
```

should show a `tun` adapter

## Show networks accessible via the VPN

```bash
netstat -rn
```