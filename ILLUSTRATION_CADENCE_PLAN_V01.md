# Illustration cadence remediation plan

## Rule
Each scene begins with its illustration, followed by the exact linked 3?4 sentence text group. Every scene receives a stable ID, paragraph start/end anchors, and an existing image path before publication.

## Audit
- **volume-1**: 852 sentences, 264 illustrations, current 3.23 sentences/illustration; target 213?284 (nominal 244), add about 0.
- **chapters-10-19**: 1520 sentences, 90 illustrations, current 16.89 sentences/illustration; target 380?506 (nominal 435), add about 345.
- **chapters-20-29**: 1108 sentences, 108 illustrations, current 10.26 sentences/illustration; target 277?369 (nominal 317), add about 209.

## Work sequence
1. Freeze paragraph IDs and sentence boundaries from the current public text.
2. Build a scene manifest with 3?4 sentence groups and an illustration-first insertion point.
3. Generate scenes in chapter order, varying establishing, medium, close-up, object, and reaction compositions while preserving character continuity.
4. Register each image by scene ID; reject missing or duplicate paths.
5. Regenerate HTML from the manifest so image precedes its linked text.
6. Verify cadence, anchors, image existence, order, and public responses before deployment.

## Acceptance checks
- Every sentence belongs to exactly one scene group.
- Every scene has one image and one contiguous text anchor.
- No group has fewer than 3 or more than 4 sentences except a chapter boundary or deliberately isolated reveal, which must be recorded.
- The browser render is checked separately from static HTML checks.
