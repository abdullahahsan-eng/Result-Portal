Milli Model School Result Portal — updated print/status build

Files: index.html, teacher.html, cloud-config.js, logo.png.

Included changes:
- Seven marks subjects: Urdu, Maths, Hindi, English, Islamiat, Science, S.S.
- Grade-only subjects: Arabic, Home Science, Computer.
- Enter Marks has a Half-Yearly-only status selector: Present / AB (Absent) / ML (Medical Leave). No separate Unit Test marks entry is added.
- Present: enter combined marks out of 100. AB/ML: enter the available Unit Test marks out of 20; output displays e.g. 15/20 (AB) or 15/20 (ML) with blue highlight.
- AB/ML subjects count as fail for the subject and final result under the user-confirmed rule. Percentage uses counted marks over 700.
- Full class A3 landscape print: green PASS result cell, red FAIL result cell, failing subject marks red, AB/ML entries blue; larger table type and print color preservation.
- Individual report card: failing subjects red, AB/ML marks blue, PASS/FAIL status highlighted.
- CSV export includes Half-Yearly status text. CSV format cannot store cell colours, so a separate “Download Coloured Excel” export is included for colour formatting.
- Public DOB field keyboard fix retained.

Important: do not reset Supabase or replace cloud-config.js unless you intend to change project settings. Upload the updated index.html and teacher.html to the repository root. Existing Supabase records are not reset by these files. The new Half-Yearly status is stored with subject marks when saved.
