TAILOR BRIEFING — PALETTE PROPAGATION
=====================================

PARTICIPANT: Tony Taslim · Efficient Business Solutions
SCOPE: Visual-brand propagation only (colour + fonts). Do not touch voice, ICP, or positioning copy in this pass.

CANONICAL SOURCE (single source of truth):
  tony-taslim-context.md → "Colours (CANONICAL …)" block, and brand-os-tony-taslim.html :root variables.
  Every other skill imports these values; none redefines them locally.

CONFIRMED PALETTE:
  Ink Charcoal   #16302B  — anchor / dark backgrounds / body text on light
  Deep Teal      #0F6E56  — primary brand presence (accents, underlines, badges, dividers, key numbers)
  Signal Amber   #BA7517  — SINGLE action colour only (CTAs, key figures). Never body text. Fails AA on paper at body size (3.42:1)
  Slate Teal     #5E736B  — secondary text, borders, dividers, captions. Replaces opacity-muted text and all ad-hoc local greys. AA 4.66:1 on paper
  Warm Paper     #F7F5EF  — neutral base / light backgrounds
  DISTRIBUTION: 60% paper+ink, 30% teal, 10% amber

FONTS:
  Playfair Display (display/headings) · Poppins (body) · DM Mono (numbers/labels)

BANNED IN ANY EBS OUTPUT (Purely Personal template defaults — vendor brand, not Tony's):
  #e90d41 (red) · #f7f7f8 (off-white) · #0a0a0a (near-black) · Rethink Sans · Inter · JetBrains Mono

FILES TO REWRITE (palette + font only):

1. content-strategy/references/design-system.md
   - Replace ad-hoc neutrals #4A554F, #E4E1D8, #EFEDE4 with Slate Teal #5E736B.
   - Reconcile #0B5443/#2E9077 (teal tints) to derive from #0F6E56; keep only if used as hover/dark states, else remove.
   - Remove semantic reds/greens (#9A3B2E) unless genuinely status-only.

2. linkedin-caption-writer/references/design-system.md
   - Add Slate Teal #5E736B as secondary/muted.
   - Remove #16A34A, #D97706, #DC2626 unless strictly status semantics; amber is #BA7517, not #D97706.

3. newsletter-writer/references/design-system.md
   - Add Slate Teal #5E736B as secondary/muted. Confirm core four match canonical exactly.

4. marketing-designer (references)
   - It hardcodes no hex — insert an explicit instruction: "Pull all colour values from tony-taslim-context.md canonical block. Never invent hex codes." Same for font names.

5. marketing-presenter (references)
   - Same instruction as #4: bind to canonical source for both colour and fonts.

ALREADY FIXED THIS PASS (do not duplicate):
  - canva-carousel.md and canva-cheatsheet.md (used by weekly-content-engine, linkedin-carousel-builder, linkedin-cheatsheet-builder) — recoloured to EBS system + fonts.
  - brand-os-tony-taslim.html and tony-taslim-context.md — Slate Teal added, marked canonical.

OUTPUT: one zip per rewritten skill folder, per standard Tailor delivery.
