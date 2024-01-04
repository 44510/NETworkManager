---
sidebar_position: 0
---

# Next Release

Version: **Next release** <br />
Release date: **xx.xx.2023**

| File | `SHA256` |
| ---- | -------- |

**System requirements**

- Windows 10 / Server x64 (1809 or later)
- [.NET Desktop Runtime 8.0 (LTS) - x64](https://dotnet.microsoft.com/en-us/download/dotnet/8.0/runtime)

## Breaking Changes

## What's new?

- Run Command
  - Run command (HotKey: Ctrl+Shift+P) added. This feature allows you to open a command field to switch between applications (and pass parameters to them _in the future_) [#2577](https://github.com/BornToBeRoot/NETworkManager/pull/2577)
- IP Scanner
  - NetBIOS resolver added to enhance the detection of hosts (e.g. if there is no ICMP response or TCP port is open) but netbios responds. It will also display the Computername if no DNS hostname is available. [#2590](https://github.com/BornToBeRoot/NETworkManager/pull/2590)
- Ping Monitor
  - UI redesigned [#2573](https://github.com/BornToBeRoot/NETworkManager/pull/2573)
  - Allow ranges like `192.168.0.0/24` or `10.0.[0-255].1` [#2573](https://github.com/BornToBeRoot/NETworkManager/pull/2573)
- Connections
  - Resolve remote hostname, process id, process name and process path (similar to `netstat`) [#2587](https://github.com/BornToBeRoot/NETworkManager/pull/2587)

## Improvements

- IP Scanner
  - Scan is no longer aborted if the IP of a single host in a series of hosts cannot be resolved (the host is skipped and an error is displayed) [#2573](https://github.com/BornToBeRoot/NETworkManager/pull/2573)
  - Sort by IP address & MAC address improved / fixed [#2583](https://github.com/BornToBeRoot/NETworkManager/pull/2583)
- Port Scanner
  - Scan is no longer aborted if the IP of a single host in a series of hosts cannot be resolved (the host is skipped and an error is displayed) [#2573](https://github.com/BornToBeRoot/NETworkManager/pull/2573)
  - Hostname added to group [#2573](https://github.com/BornToBeRoot/NETworkManager/pull/2573)
  - Sort improved [#2583](https://github.com/BornToBeRoot/NETworkManager/pull/2583)
  - Port profile column sort fixed [#2583](https://github.com/BornToBeRoot/NETworkManager/pull/2583)
- Ping Monitor
  - Scan is no longer aborted if the IP of a single host in a series of hosts cannot be resolved (the host is skipped and an error is displayed) [#2573](https://github.com/BornToBeRoot/NETworkManager/pull/2573)
- DNS Lookup
  - Hostname of the nameserver added to group [#2573](https://github.com/BornToBeRoot/NETworkManager/pull/2573)
  - Sort improved [#2583](https://github.com/BornToBeRoot/NETworkManager/pull/2583)
- SNMP
  OID profile column sort fixed [#2583](https://github.com/BornToBeRoot/NETworkManager/pull/2583)
- Connections
  - Sort by IP address improved / fixed [#2583](https://github.com/BornToBeRoot/NETworkManager/pull/2583)
- Listeners
  - Sort by IP address improved / fixed [#2583](https://github.com/BornToBeRoot/NETworkManager/pull/2583)
- ARP Table
  - Sort by IP address & MAC address improved / fixed [#2583](https://github.com/BornToBeRoot/NETworkManager/pull/2583)

## Bugfixes

- SNMP
  - Detect EndOfMibView in v1 and v2c walk [#2583](https://github.com/BornToBeRoot/NETworkManager/pull/2583)
- Lookup
  - Fix sort by MAC address [#2583](https://github.com/BornToBeRoot/NETworkManager/pull/2583)

## Dependencies, Refactoring & Documentation

- Code cleanup & Refactoring [#2583](https://github.com/BornToBeRoot/NETworkManager/pull/2583) [#2586](https://github.com/BornToBeRoot/NETworkManager/pull/2586)
- Language files updated [#transifex](https://github.com/BornToBeRoot/NETworkManager/pulls?q=author%3Aapp%2Ftransifex-integration)
- Dependencies updated [#dependencies](https://github.com/BornToBeRoot/NETworkManager/pulls?q=author%3Aapp%2Fdependabot)