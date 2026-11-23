# LIVE WIRE TICKET™ — Exact Imagery & Production Schema (Nov 23, 2026)

A drop-in handoff spec for reproducing the exact Token coins, 9:16 Broadsheet Newspapers, Landscape Ticket Faces, and 1080×1920 Spin Videos across all 8 houses.

## 1. Global Color Canon & Schemes

| Token / Scheme | Exact Values / Rules |
|---|---|
| wire-pink-teal | Left edge: #ec4899 (hot pink) · Right edge: #14b8a6 (teal) |
| full-gold | Brushed/crinkled gold foil (#d4af37 / #f5df86 / #9c7216), dark ink #1c1404 |
| marble-gold-silver | White marble (#fcfbf8–#f3efe7), gold foil trim, silver-platinum center, diffuse tie-dye pink/teal veining (wide, soft, low-density) |
| whited-silver-brass | Silver/platinum (#e5e7eb–#cbd5e1) with brass/champagne (#b89b5e), old-world fine crisp lines |
| Background Canvas | Matte charcoal-black #0a0b0f (with subtle #ec4899 left / #14b8a6 right ambient rim glow) |
| Status Colors | NOT SETTLED — do not lock blue vs. yellow for status without Garrett's word |

## 2. House Registry (No. 0001 – No. 0008)

| No. | House / Issuer (Lower Ring) | Center Mark | Center Emblem | Left Inlay | Right Inlay | Metal Finish |
|---|---|---|---|---|---|---|
| 0001 | MY AI ASSISTANCE OFFICE | THE AI OFFICE | Brass key + single rose | #ec4899 (Pink) | #14b8a6 (Teal) | Solid Gold |
| 0002 | BUMKUS (Vice City Wire) | VICE CITY WIRE | Open bridge / sunset palms | #ec4899 (Pink) | #14b8a6 (Teal) | Gold rim / Silver-platinum center |
| 0003 | BUMKUS STUDIOS | THE CATALOG | 4 geometric containers + rose | #1f2430 (Black) | #c0c7d6 (Silver) | Brass rim / Brushed-silver center |
| 0004 | AI GOVERNANCE OFFICE | ECHOLUS | Balance scale + verified shield | #132a63 (Navy) | #00c8c8 (Teal) | Solid Gold |
| 0005 | BUMKUS NOTES | MANAGER NOTES | Fountain pen nib + ledger page | #facc15 (Yellow) | #1d4ed8 (Cobalt) | Solid Gold |
| 0006 | BUMKUS SPORT | EVIE • GYMFLOW | Championship medal + ribbon | #7e22ce (Purple) | #18181b (Black) | Solid Gold |
| 0007 | BUMKUS BOTANICALS | CLEAR • GROUNDED | Botanical leaf sprig + drop | #047857 (Emerald) | #e7d5a8 (Cream) | Solid Gold |
| 0008 | BUMKUS IP LAB | LICENSING | Classic rose + wax-seal key | #991b1b (Crimson) | #111827 (Black) | Solid Gold |

## 3. The Token (Coin) — Exact Spec & Prompt Template

- Aspect Ratio & Resolution: 1:1 (1024×1024 master)
- Anatomy (Outside → Inside):
  1. Finely milled metallic outer rim (~3% radius).
  2. Curved enamel inlay arcs: Left arc = Left Inlay, Right arc = Right Inlay.
  3. Engraved ring text: Upper arc = LIVE WIRE TICKET™, Lower arc = {HOUSE_LOWER_RING}.
  4. Recessed brushed-metal center medallion (~68% diameter) with dark-engraved {EMBLEM}, {CENTER_MARK}, and No. {NNNN}.
- Exact Prompt Template: [template body did not come through in the paste — Nov 23]

## 4. The Newspaper (Broadsheet) — Exact Spec & Prompt Template

- Aspect Ratio & Resolution: 9:16 (1080×1920 video-ready; 768×1376 AI still base)
- Anatomy (Top → Bottom):
  1. Outer Border: Dark black background with a glowing rounded-rectangle neon border (#ec4899 pink on left fading to #14b8a6 teal on right).
  2. Paper: Weathered, slightly creased cream newsprint sheet centered inside the neon frame.
  3. Top Banner & Masthead: Small Art Deco banner (EST. 2026) above bold vintage serif masthead ({HOUSE_MASTHEAD}).
  4. Subheader Rule: Thin horizontal rule with diamond accents: THE DAILY WIRE - No. {N} - {LOCATION}.
  5. Headline: Bold condensed black serif all-caps ({HEADLINE}).
  6. Centerpiece Illustration: Art Deco rectangular frame with radiating corner sunburst lines; detailed vintage ink-engraving with subtle #ec4899 pink (left) and #14b8a6 teal (right) neon highlights.
  7. Body Copy & Footer: Crisp black serif editorial copy, followed by {DOMAIN} - {TAGLINE} and licensing line (© 2026 Bumkus, licensed, never sold).
- Exact Prompt Template: [template body did not come through in the paste — Nov 23]

## 5. Landscape Ticket Face & Plug-In Contract

- Plug-In Contract: SURFACE (given) → SCHEME MASK (ours) → PIECE (content). Always build from a blank copy of the template, never on the base. Frame-exact; slot contracts at 150 DPI.
- Canvas Placement: Landscape ticket face centered on 1080×1920 vertical canvas over a blur-fill of itself.
- Required Elements:
  - Masthead (THE DAILY WIRE / {HOUSE_MASTHEAD}) + Headline
  - GOLDEN TICKET designation + No. {NNNN}
  - Perforation line + notched ADMIT ONE stub + decorative barcode
  - Microprint: VALID FOR ONE PERSON - DOORS 7PM - SHOW 8PM - NO REFUNDS
  - Left edge #ec4899 pink, right edge #14b8a6 teal, gold foil trim
  - Back Card (Closing): THE WIRE CARRIED IT LIVE · No. {NNNN} · FOLLOW {HANDLE} · PASS THIS TICKET ON

## 6. Video & 3D Spin Pipeline (1080×1920, 30 fps, H.264 yuv420p)

- 3D Coin Spin:
  - Extract circular coin with smooth radial alpha mask.
  - Y-axis rotation theta = 2π * (frame / total_frames): horizontal scale |cos(theta)|, 3D milled gold edge extrusion thickness = 38px * |sin(theta)|, dynamic specular sweep across X, and soft floor shadow scaling with |cos(theta)|.
  - Reverse face (cos(theta) < 0): brushed gold with pink/teal enamel arcs, THE WIRE CARRIED IT LIVE, No. {NNNN}, and {HOUSE_LOWER_RING}.
- 7-Beat Coin-Opener Play:
  1. Coin sits on Daily Wire page → 2. Shadow sweep → 3. Coin falls into place → 4. Rolls off → 5. Turns gold-to-marble → 6. Opens → 7. Content video plays inside.
- Ticket Wire-In Play: ~2s slow push-in on Face → 0.35s white-flash amperage cut → full Content → ~2s Back card.
- Audio Rule (Nov 23): No synthesized audio — real sound only. Quiet tension music bed underneath; per-segment gain staging (never a single whole-program loudnorm).
