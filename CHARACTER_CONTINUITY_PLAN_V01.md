# Character and style continuity plan

## Audit result

- Existing approved reference pool: `illustrated/graphic/when_you_trap_a_tiger/scenes/` with 264 PNG images from the published Chapter 1–6 reader.
- Existing machine-readable character bible: not found.
- Existing style bible: not found.
- The discarded Chapter 10 batch was generated without an approved reference-bible gate and is removed from the public site.

## Required resources before new generation

1. **Character bible**: Lily, Sam, Mom, Halmoni, the female tiger, Joe, Jensen, Ricky, Rick, Olivia, and embedded-tale characters. Each entry must specify age/role, face shape, hair, eyes, skin tone, body proportions, wardrobe by period/scene, fixed props, and forbidden changes.
2. **Style bible**: line quality, palette, lighting, background simplification, camera language, panel composition, crop rules, and the exact 4×4 grid layout.
3. **Reference board**: select approved existing images for each recurring character and location. References come from the published Chapter 1–6 pool; generated images cannot become references until reviewed.
4. **Continuity ledger**: record scene ID, character IDs, wardrobe state, props, location, time, reference image IDs, prompt, grid batch ID, reviewer result, and public asset path.

## Generation gate

- No new image generation until the character bible, style bible, and reference board are approved.
- Every batch is exactly one 4×4 grid with 16 distinct panels.
- Every panel must preserve the character IDs and state recorded in the ledger.
- Reject a batch when face, hair, clothing, proportions, palette, line treatment, or setting drifts from the approved references.
- Split and register all 16 cells only after visual review; unreviewed cells are not published.

## Sequence

1. Build the bible and reference board from the 264 approved Chapter 1–6 images.
2. Validate the bible against at least three existing images per recurring character and two per recurring location.
3. Rebuild Chapter 10 scene batches with reference images attached to every generation request.
4. Review one 4×4 grid before producing the next grid.
5. Register the 16 cells, place the illustration before its linked 3–4 sentence text group, run static and visual checks, then publish.
6. Repeat chapter by chapter through Chapter 29.

## Acceptance criteria

- Character identity matches the approved reference board across all 16 cells.
- The same character's hair, face, clothing, and prop state do not change without a ledgered story event.
- Every cell has a scene ID, text anchor, image file, and review record.
- No placeholder or unreviewed image reaches the public site.
