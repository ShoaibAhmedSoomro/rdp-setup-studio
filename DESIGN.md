# RDP Setup Studio, design notes

Audience: a completely non-technical person. Job: get them to a working cloud Windows desktop without needing to understand GitHub, Tailscale or YAML.

## Decisions (v3)
- Plain words over metaphor. The v2 "cable and ports" concept was dropped: "port seated" and "touches GitHub" meant nothing to a beginner. Steps are just "Step 3 of 9" with a time estimate.
- One action per numbered line, with a small grey "why" or "where to look" line under it when needed.
- Every step explains its one technical word in a sentence (project folder, key = invitation, secret = locked box).
- Only 4 questions up front (GitHub username, Windows name, project name, password choice). Everything else sits under "More options" with sensible defaults, and opens by itself if one of its answers is invalid.
- The setup-file code is hidden behind "The editor opened empty?" since most people never need to see it.
- Phones: one column, the "Your setup" card drops below, Back/Continue stay pinned to the bottom with the status line above them.
- Still page by decision: no idle animation. Motion is limited to a short fade-in per step, progress bar fills and control feedback, all off under reduced motion.

## System
Palette (light / dark): ground #F5F6F8 / #0E1116, panel #FFFFFF / #161B22, ink #121722 / #E8ECF1, muted #576071 / #9AA4B2, accent #2153D1 / #7C9DFF, done #127A4B / #4CC58E, caution #8A4F00 / #F2B155.
Type: Archivo for everything, IBM Plex Mono only for things people copy or type exactly.
Shape: 14px panels, 10px buttons and notes, 6px small controls. Tap targets 48px on inputs and buttons.
