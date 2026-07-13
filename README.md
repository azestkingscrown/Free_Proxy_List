# Free Active Proxy List

This repository provides a continuously validated list of active public proxies, automatically verified and updated every half hour.

## Features

- **Half-Hourly Updates**: Automatically tested and updated every half hour.
- **Pre-Filtered**: Invalid, dead, or extremely slow proxies are discarded.
- **Multiple Formats**: Provided in both a simple list (`working_proxies.txt`) and a detailed JSON with latency statistics (`proxy_stats.json`).

## Motivation & Purpose

Free proxy lists published on the internet are notorious for having a short lifespan. Most public IPs get blocked or go offline within minutes or hours. 

This repository was created to automatically parse public lists, perform concurrent health and latency checks, and publish only the active and functional proxies (primarily SOCKS5). It ensures that developers have immediate access to a clean, ready-to-use list of working proxies without having to test thousands of dead ones manually.

## Tool & Source Code

The validation and deployment tool used for this repository is written in Go and is open-sourced here:
- **Go Proxy Checker Repository**: [azestkingscrown/free-proxy-checker](https://github.com/azestkingscrown/free-proxy-checker)

## Upstream Data Sources

The raw proxy data is aggregated and scraped from multiple public sources:
- [proxifly/free-proxy-list](https://github.com/proxifly/free-proxy-list)
- [TheSpeedX/PROXY-List](https://github.com/TheSpeedX/PROXY-List)
- [komutan234/Proxy-List-Free](https://github.com/komutan234/Proxy-List-Free)
- [stormsia/proxy-list](https://github.com/stormsia/proxy-list)

## Acknowledgments

Special thanks to the creators and contributors of the open-source projects above for collecting, maintaining, and aggregating the raw proxy lists used by this validation tool.

---

*Note: This repository is updated programmatically using an automated Go-based checker script.*
