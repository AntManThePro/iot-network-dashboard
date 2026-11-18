# IoT Network Dashboard

A scan-file viewer for the IoT network analysis workflow. Drop in your scan outputs and it turns them into something you can actually read — summary stats, a searchable host inventory with ports and services, high-risk port flags, and a diff against your baseline. Built by DoubleA (@AntManThePro). Not perfect, just real.

**Live:** https://iot-network-dashboard.netlify.app/

## How to use it

1. Run the scan scripts on a machine on your LAN first (`master.sh` in the iot-analysis workflow) — this page does not scan, a browser can't run nmap or ARP.
2. Open the live site and drop in the output files: `profile_*.xml`, `hosts_*.gnmap`, `live_hosts.txt`, `baseline.json`, `report_*.txt` — or the whole folder.
3. Browse the host inventory, check the high-risk port flags (Telnet, SNMP, UPnP, plain MQTT, HTTP admin), and compare against a baseline to see what changed.
4. Download or copy the regenerable report when you're done.

It starts empty — no sample hosts, no made-up data.

## What it flags

- High-risk ports: Telnet, SNMP, UPnP, plain MQTT, HTTP admin
- Changes diff against `baseline.json` or an older scan
- Searchable host inventory with ports and services

## Links

- Live site: https://iot-network-dashboard.netlify.app/
- NEXUS hub: https://nexus-world-hub.netlify.app/
- Repo: https://github.com/AntManThePro/iot-network-dashboard

## Deploy

Single-file app plus icon set. Publish root, no build command, branch main.
