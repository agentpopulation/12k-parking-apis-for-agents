## Parking API endpoints, snapshot 15 Nov 2026

- 12,327 endpoints passed a keyless data call, tested 11–15 Nov 2026 (IST)
- 3,189 services · 59 country codes · 10,126 keyless JSON rows

### Download

- `Parking_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 12,327 rows, 674.3 kB gzipped (4.1 MB as CSV), SHA-256 `dec3c86673cf2374e323d78d08e47d0c3dbe8986257b469110812b5316108a98`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Parking_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Parking_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 7,540 · Wrap one URL pattern as a find_parking tool: pass a city or a point, return nearby car parks or zones with capacity, occupancy where the source gives it, and the time of the reading.
- 📱 App features: 3,266 · Draw car parks, garages, on-street zones, meters and accessible bays on a map, and show capacity, tariff or opening hours where the layer has them.
- 🧠 Grounding and data pipelines: 2,536 · Load car-park tables, occupancy history and parking-ticket records on a schedule into your own store, so answers about parking supply and demand cite a dated source.
- 🧪 Evals and testing: 12,327 · Run your parking tool against a fixed set of URLs across formats; check that name, location, capacity, occupancy and time parse, and keep last_tested as the baseline for your own re-tests.

### Changes

- First release
- Left out: 177 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 2 layers marked editable in the title (they can hold entries that people added).
- Left out: 21 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 98 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 19 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Left out: 7 rows of server information from Mastodon, PeerTube, Lemmy, Nostr and other social network servers (instance documents name the server's contact person).
- Overlap: 104 of these URLs are also in 190k-weather-apis-for-agents.
- Overlap: 12,327 of these URLs are also in 270k-transit-apis-for-agents.
- Overlap: 114 of these URLs are also in 270k-water-apis-for-agents.
- Overlap: 13 of these URLs are also in 130k-finance-economy-apis-for-agents.
- Overlap: 29 of these URLs are also in 130k-india-apis-for-agents.
- Overlap: 846 of these URLs are also in 1.3m-government-open-data-apis.
- Overlap: 5 of these URLs are also in 86k-oceans-apis-for-agents.
- Overlap: 60 of these URLs are also in 24k-maritime-apis-for-agents.
- Overlap: 1 of these URLs is also in 170k-environment-apis-for-agents.
- Overlap: 1 of these URLs is also in 20k-air-quality-apis-for-agents.
- Overlap: 146 of these URLs are also in 380k-maps-gis-apis-for-agents.
- Overlap: 10,126 of these URLs are also in 2.5m-agent-ready-apis.
- Overlap: 1 of these URLs is also in 96k-health-apis-for-agents.
- Overlap: 39 of these URLs are also in 53k-hazards-apis-for-agents.
- Overlap: 26 of these URLs are also in 25k-aviation-apis-for-agents.
- Overlap: 120 of these URLs are also in 24k-traffic-apis-for-agents.
- Overlap: 1 of these URLs is also in 5.2k-volcano-tsunami-apis-for-agents.
- Overlap: 3 of these URLs are also in 17k-bike-share-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 11–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Parking API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
