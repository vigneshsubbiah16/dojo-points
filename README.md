# 🥋 Dojo Bros — family dojo points

ClassDojo-style points for Niranjan & Nikhilan, hosted free on GitHub Pages.

**Live app:** https://vigneshsubbiah16.github.io/dojo-points/

## How it works

- The repo itself is the database: every award/redeem is a commit to `state.json`.
- Anyone with the link (the kids) sees points, belts, streaks, badges, rewards, and history — read-only.
- Parents unlock **parent mode** to give points, redeem rewards, and edit behaviors/rewards.

## One-time parent setup

1. Create a **fine-grained personal access token** at
   https://github.com/settings/personal-access-tokens/new
   - Repository access: **only this repo** (`dojo-points`)
   - Permissions: **Contents → Read and write**
   - Expiration: 1 year (set a reminder to rotate)
2. Open the app → **🔒 Parent** → paste the token → **set a family password**.
3. On any other device (wife's phone, etc.): **🔒 Parent** → type the family password. Done.

The family password decrypts the token (AES-GCM, encrypted blob in `vault.json`) —
no server, no accounts. Kids' devices never need it.

## Belts

Lifetime points earn belts: White → Yellow (25) → Orange (60) → Green (100) →
Blue (160) → Purple (240) → Brown (340) → Red (460) → Black (600).
