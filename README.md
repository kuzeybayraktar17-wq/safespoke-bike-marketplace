# SafeSpoke – checking secondhand bikes before you buy

Course project for GUI Design & Web Optimization (Cycle 1, Personal Product).

**Brief:** *Secondhand bike marketplace.* A student wants to buy a reliable used bike without getting scammed or ending up with a stolen one, while there's no easy way to check a listing is trustworthy.

## Versions
- **v2 (current):** [`/v2/`](v2/), redesigned after the heuristic self-evaluation, desk research and two user interviews.
- **v1 (Week 1):** [`/`](index.html), the first one-shot AI build.

## What v2 does
0. **Is a bike worth it?** Compares a used bike with what you pay per trip now (e.g. scooter rides).
1. **Check a listing:** five questions, one per step with a progress bar. The result is a label plus reasons and a next action for each warning. There is no number score.
2. **Ask the seller:** copy-ready messages in German and English (frame number, receipt, paying in person, meeting place).
3. **Meeting mode:** a handover checklist. Progress is saved on the device and can be reset.
4. **Purchase record:** a simple "Kaufvertrag" with the frame number, to show, print or photograph.

## What changed from v1, and why
| v1 problem | Source | v2 change |
|---|---|---|
| Verdict shown after the first answer | Heuristic eval: visibility of system status | Step-by-step check with progress; the result only appears at the end |
| 0–100 score looked more exact than it is | Heuristic eval: match with the real world | Label and reasons only |
| No Reset or Clear; checklist lost on reload | Heuristic eval: user control | Reset buttons; checklist saved on the device |
| Asking for proof feels awkward | Context mapping (principles) and Kleinanzeigen tips | Message templates |
| No proof after buying | Kleinanzeigen / ADFC recommend a contract | Purchase record |
| Payment scams | Verbraucherzentrale | Payment step and checklist item |
| Cost vs. need was the real barrier; a bike was seen as 1000+ € next to 3–5 € scooter rides | Interviews 1 + 2 | "Is a bike worth it?" calculator |
| People ask for an invoice and warranty but never the frame number | Interviews 1 + 2 | Proof step checks the name and frame number on the invoice |
| Theft worry comes after buying (AirTag, "wouldn't leave it outside") | Interview 1 | "Protect your bike" screen |

Static HTML/CSS/JS with no dependencies and no tracking. Data stays in the browser.

Built with an AI code agent (Claude) and based on my own research and evaluation.
