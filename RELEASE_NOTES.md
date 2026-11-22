## Traffic and roadworks API endpoints, snapshot 15 Nov 2026

- 22,827 endpoints passed a keyless data call, tested 10–15 Nov 2026 (IST)
- 2,519 services · 220 country codes · 12,593 keyless JSON rows

### Download

- `Traffic_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 22,827 rows, 1.1 MB gzipped (6.9 MB as CSV), SHA-256 `de8cd967e4227e4ae3a550c870aaa27a8a12d465bcb8956e9fba76fa693fe2a5`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Traffic_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Traffic_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 7,885 · Wrap one URL pattern as a get_traffic tool: pass a station id or a road area, return vehicle counts, average speed or road-surface readings with the measurement time and a timeout.
- 📱 App features: 718 · Show roadworks and closures near a route on a map card with the start and end dates each layer gives, and past crashes as a road-safety layer.
- 🧠 Grounding and data pipelines: 9,089 · Load counting-station files, crash tables and road-death rates on a schedule into your own store, so answers about traffic volumes and road safety cite a dated source.
- 🧪 Evals and testing: 22,827 · Run your traffic tool against a fixed set of URLs across formats; check that station, count, speed, location and time parse, and keep last_tested as the baseline for your own re-tests.

### Changes

- First release: 24,641 endpoints from 2,782 services, tested 10–15 Nov 2026 (IST), snapshot 15 Nov 2026.
- Rebuilt under the same snapshot with the latest leave-out rules (other addresses of a left-out ArcGIS layer, teaching organisations, more class-layer, name and record rules): 22,827 endpoints from 2,519 services, 1,814 fewer endpoints than first published under this snapshot (24,641 from 2,782 services), tested 10–15 Nov 2026 (IST).
- Left out: 4 rows with an email-like address.
- Left out: 337 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 1 layer marked editable in the title (it can hold entries that people added).
- Left out: 75 police traffic-stop layers (they can hold details of people stopped).
- Left out: 23 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 968 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 21 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Left out: 1 ArcGIS layer that is a record about named people (employee, patient, client or donor lists, home addresses, voter lists, sex offender and missing person layers).
- Left out: 10 rows of server information from Mastodon, PeerTube, Lemmy, Nostr and other social network servers (instance documents name the server's contact person).
- Left out: 18 rows of ArcGIS Online organisations that are class accounts (25 layers or more, at least 50% of them class or coursework layers): their other layers are students' work too.
- Left out: 632 rows of ArcGIS Online organisations that are class accounts (3 class sets or more in at least 20% of their rows, 10 class sets or more with no organisation name, or layers signed by students read by hand): their other layers are students' work too.
- Left out: 307 rows of class sets: one map layer saved under 5 or more students' initials or names in one ArcGIS Online organisation, or in 4 or more students' own organisations.
- Left out: 808 rows of the ArcGIS Online organisations of universities, colleges and schools (many of their layers are students' work).
- Left out: 15 rows that repeat an address already in the pack.
- Left out: 946 development-plan map services (GetCapabilities) of Villingen-Schwenningen, Germany, tagged by the German word Verkehr: not traffic data.
- Left out: 1,214 land-use tables ("settlement and traffic areas") of German municipalities: not traffic measurements.
- Left out: 643 Destatis economy, trade and enterprise tables tagged by the word Verkehr: not road traffic.
- Overlap: 276 of these URLs are also in 170k-weather-apis-for-agents.
- Overlap: 22,790 of these URLs are also in 240k-transit-apis-for-agents.
- Overlap: 1,123 of these URLs are also in 260k-water-apis-for-agents.
- Overlap: 125 of these URLs are also in 120k-finance-economy-apis-for-agents.
- Overlap: 59 of these URLs are also in 130k-india-apis-for-agents.
- Overlap: 205 of these URLs are also in 1.2m-government-open-data-apis.
- Overlap: 18 of these URLs are also in 270k-statistics-apis-for-agents.
- Overlap: 968 of these URLs are also in 84k-oceans-apis-for-agents.
- Overlap: 1,293 of these URLs are also in 22k-maritime-apis-for-agents.
- Overlap: 13 of these URLs are also in 160k-environment-apis-for-agents.
- Overlap: 30 of these URLs are also in 19k-air-quality-apis-for-agents.
- Overlap: 1,846 of these URLs are also in 350k-maps-gis-apis-for-agents.
- Overlap: 12,557 of these URLs are also in 2.2m-agent-ready-apis.
- Overlap: 133 of these URLs are also in 84k-health-apis-for-agents.
- Overlap: 61 of these URLs are also in 380k-science-apis-for-agents.
- Overlap: 77 of these URLs are also in 40k-hazards-apis-for-agents.
- Overlap: 15 of these URLs are also in 67k-energy-apis-for-agents.
- Overlap: 1,024 of these URLs are also in 23k-aviation-apis-for-agents.
- Overlap: 114 of these URLs are also in 10k-parking-apis-for-agents.
- Overlap: 1 of these URLs is also in 7.8k-earthquake-apis-for-agents.
- Overlap: 13 of these URLs are also in 17k-bike-share-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 10–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Traffic and roadworks API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
