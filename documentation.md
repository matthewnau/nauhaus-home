# Documentation

## Port Registry

| Web (HTTP / HTTPS) | Functional (P2P / Listen) | Category / Purpose                        |
| :----------------- | :------------------------ | :---------------------------------------- |
| `10000`–`10099`    | `20000`–`20099`           | Security / Networking (VPNs, Ad Blocking) |
| `10100`–`10199`    | `20100`–`20199`           | Download / P2P (qBittorrent, Soulseek)    |
| `10200`–`10299`    | `20200`–`20299`           | Media Processing (MKVToolNix, Filebot)    |
| `10300`–`10399`    | `20300`–`20399`           | Media Servers (Plex, Jellyfin)            |
| `10400`–`10499`    | `20400`–`20499`           | Development / Sandbox                     |

## Service Registry

| Category              | Service / Container | Image                           | Web Port | Functional Ports |
| :-------------------- | :------------------ | :------------------------------ | :------- | :--------------- |
| Security / Networking | `gluetun-c01`       | `qmcgaw/gluetun`                | —        | —                |
| Download / P2P        | `qbittorrent-c01`   | `linuxserver/qbittorrent`       | `10100`  | `20100`          |
| Download / P2P        | `soulseek-c01`      | `slskd/slskd`                   | `10110`  | `20110`          |
| Media Processing      | `mkvtoolnix-c01`    | `jlesage/mkvtoolnix`            | `10200`  | —                |
| Media Processing      | `mkvtoolnix-c02`    | `jlesage/mkvtoolnix`            | `10210`  | —                |
| Media Processing      | `filebot-c01`       | `jlesage/filebot`               | `10220`  | —                |
| Development / Sandbox | `server-c01`        | `halverneus/static-file-server` | `10410`  | —                |