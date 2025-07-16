⚠️ No UPnP-enabled router found
You will need to manually forward port 8003:
1. Access your router settings
2. Add port forwarding rule:
   - External Port: 8003
   - Internal IP: 172.20.167.56
   - Internal Port: 8003
   - Protocol: TCP

ℹ️ Your node will still work, but requires manual port forwarding.
No updates available. You are on version 0.2.8.
Node is already registered; skipping new registration.
FileCache loaded 0 existing entries from disk.
Error: Os { code: 98, kind: AddrInUse, message: "Address already in use" }
phamhung@Hungda:~$ ./pop --status
Found existing /home/phamhung/node_info.json. Attempting to parse...
Parsed node_info.json => node_id=7648e332-49cc-4167-82de-ecb36aa08eb0, registered=true

==============================================
  🚀 Reputation Status for Node: 7648e332-49cc-4167-82de-ecb36aa08eb0
==============================================
  Uptime Score:        1.000
  Egress Score:        0.000
  Historical Score:    1.000
----------------------------------------------
  TOTAL SCORE:         0.700  ✅
==============================================

phamhung@Hungda:~$
