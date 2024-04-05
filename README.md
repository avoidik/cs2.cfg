# CS2 Custom Configuration

To enable this configuration:
1. Change `CS2_MAPGROUP` to `mg_allmaps`
2. Change `CS2_CFG_URL`to `https://github.com/avoidik/cs2.cfg/releases/download/v1.0.0/config.tar.gz`

For example:

```terminal
$ docker run -d --name=cs2 \
    -e SRCDS_TOKEN="$SRCDS_TOKEN" \
    -e CS2_CFG_URL="https://github.com/avoidik/cs2.cfg/releases/download/v1.0.0/config.tar.gz" \
    -e CS2_MAPGROUP="mg_allmaps" \
    -p 27015:27015/tcp \
    -p 27015:27015/udp \
    joedwards32/cs2
```

# References

- [Steam token](https://steamcommunity.com/dev/managegameservers)
- [joedwards32/CS2](https://github.com/joedwards32/CS2)
- [Game Modes](https://developer.valvesoftware.com/wiki/Counter-Strike:_Global_Offensive/Game_Modes)
