# docker-openvpn-setup

setup and config scripts for openvpn on docker

## Usage

Setup OpenVPN Docker container and run OpenVPN server

```bash
curl -fLo setup https://raw.githubusercontent.com/b-ggs/docker-openvpn-setup/master/setup
chmod +x setup
ADDRESS=xxx.xxx.xxx.xxx ./setup
# Where ADDRESS is the VPS's IPv4 address
```

Generate client and OVPN config

```bash
curl -fLo generate_client https://raw.githubusercontent.com/b-ggs/docker-openvpn-setup/master/generate_client
chmod +x generate_client
CLIENT_NAME=client ./generate_client
# Where CLIENT_NAME is the client name to be created
```

## Credits

* Kyle Manna's OpenVPN Docker image ([kylemanna/openvpn][dockerhub])

[dockerhub]: https://hub.docker.com/r/kylemanna/openvpn/
