# IoT Network Dashboard

A scan-file viewer for the IoT network analysis workflow in `workspace/iot-analysis/`.

Drop in profile_*.xml, hosts_*.gnmap, live_hosts.txt, baseline.json, report_*.txt (or the whole folder). It parses them on-device into summary stats, a searchable host inventory with ports/services, high-risk port flags (Telnet, SNMP, UPnP, plain MQTT, HTTP admin), a Changes diff against baseline.json or an older scan, and a regenerable report to download or copy.

It starts empty — no sample hosts. It does not scan: a browser cannot run nmap or ARP. Run the scripts on a machine on your LAN first, then load their outputs here.

## Deploy

Single-file app plus icon set. Publish root, no build command, branch main.
