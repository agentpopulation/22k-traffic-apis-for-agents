# Changelog

## 2026-11-15 (snapshot-2026-11-15)

- First release: 24,641 endpoints from 2,782 services, tested 10–15 Nov 2026 (IST), snapshot 15 Nov 2026.
- Rebuilt under the same snapshot with the latest leave-out rules (other addresses of a left-out ArcGIS layer, teaching organisations, more class-layer, name and record rules): 22,827 endpoints from 2,519 services, 1,814 fewer endpoints than first published under this snapshot (24,641 from 2,782 services), tested 10–15 Nov 2026 (IST).
- The repository holds a 1,000-row sample and the services list; the full list is the release download Traffic_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz.
- GitHub name: 22k-traffic-apis-for-agents (was 24k-traffic-apis-for-agents; first published as traffic-api-endpoints). The name follows the count, rounded down.
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
