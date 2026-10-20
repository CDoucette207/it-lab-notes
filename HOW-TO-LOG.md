# How I Log Each Week

About 20–30 minutes, same day every week (e.g. Sunday night).

## 1. Collect during the week (30 seconds at a time)
- Screenshot anything that works or breaks (Mac: **Cmd + Shift + 4**). Save into a `to-log` folder on the Desktop.
- Jot quick notes in Apple Notes: topic studied, hours, practice test scores, anything that confused you.

## 2. Write the weekly entry (10–15 min)
1. Open `study-log/2026.md`.
2. Copy `templates/weekly-entry.md` and paste it at the top of the log, under the line.
3. Fill it in from your notes: hours, topics, labs, scores.
4. Write **"One thing that clicked"** in your own words. This is the study part: if you can't explain it, review it.
5. Add one row to the summary table at the top.

## 3. Update a project write-up (only if you built something)
1. Finished a Packet Tracer phase or home lab change? Copy `templates/project-writeup.md` or update `packet-tracer/README.md` / `home-lab/README.md`.
2. Move screenshots from `to-log` into that project's `screenshots/` folder with clear names (`ospf-neighbors.png`, not `Screenshot 2026-10-20…png`).
3. Add any problem you hit to the **Problems and fixes** table.

## 4. Scrub before you commit (1 min)
- No passwords, API keys, private SSH keys, public IPs, Wi-Fi names.
- **Nothing from BIW or any employer.** Personal lab only.

## 5. Commit and push (2 min)
**GitHub Desktop:** write a summary like `Week of Oct 20: subnetting + Phase 4 OSPF` → **Commit to main** → **Push origin**.

**Terminal:**
```bash
cd ~/it-lab-notes
git add .
git commit -m "Week of Oct 20: subnetting + Phase 4 OSPF"
git push
```

## 6. Share the big ones (optional, 5 min)
Finished a phase or passed an exam? Post 3–4 sentences + one screenshot on LinkedIn and link the write-up. Update the LinkedIn project description too.

## Monthly (first Sunday)
- Update "Current focus" in the main `README.md`.
- Update the phase status table in `packet-tracer/README.md`.
