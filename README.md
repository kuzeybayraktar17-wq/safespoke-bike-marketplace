# SafeSpoke – trustworthy secondhand bikes

Cycle 1 assignment (GUI Design & Web Optimization): a one-shot, AI-built app for a randomly drawn design brief.

**Brief:** *Secondhand bike marketplace.* A student wants to buy a reliable used bike without getting scammed or ending up with a stolen one, while there's no easy way to check a listing is trustworthy.

## What it does
- **Browse bikes:** every listing shows a trust rating and the concrete reasons behind it (no black-box score). Filter by type and price, sort by trust.
- **Check a listing:** answer a few questions about any outside listing and get a plain-language verdict plus what to do next.
- **Meeting checklist:** a tick-off list for the in-person handover (frame number, proof of ownership, test ride, safe payment).

All listings are fictional demo data. It is a single static `index.html` with no dependencies and no data collection.

## Design notes
- Trust is explained, not just scored: each badge has an icon + text, never color alone.
- 44px minimum touch targets, keyboard-accessible tabs and dialog, visible focus, reduced-motion respected.
- Mobile-first layout, since the meeting checklist is meant to be used on a phone.

## Process
Built with an AI code agent (Claude) from a single prompt based on the drawn brief; see the Progress Log for details.
