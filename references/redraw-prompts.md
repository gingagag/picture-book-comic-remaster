# Panel redraw and correction guide

## Visual target

Recreate each source panel as a clean, high-resolution children's picture-book illustration. Preserve the original composition and story action while using:

- clean ink-like contours, clear color blocks, and smooth edges;
- visible rice-paper, watercolor, paper-cut, and restrained Chinese decorative texture;
- a gentle palette centered on warm cream, ochre red, indigo, blue-green, and golden orange;
- soft, playful, Chinese-myth or folk-tale warmth rather than photorealism;
- stable character proportions, clothing colors, hairstyles, and facial language across the sequence.

## Base generation prompt pattern

For each panel, explicitly describe:

1. Panel role and aspect ratio.
2. Foreground characters, poses, gaze, hands, clothing, and emotional beat.
3. Background setting, important props, and negative-space needs.
4. Continuity constraints inherited from adjacent panels.
5. Style target from the section above.
6. Exclusions: no text, letters, punctuation, numbers, captions, speech bubbles, page borders, watermarks, logos, or red markup.

Do not rely on a generic phrase such as “same as source.” State the concrete visual facts that must survive the redraw.

## Continuity rules

- A transformed or frozen character must retain that state until the story event that reverses it.
- A character's hair shape, parting, clothing, size relationship, and signature colors must remain recognizable.
- Keep entrance direction, pursuit direction, embrace direction, and other spatial logic consistent between adjacent panels.
- Do not add a new character, prop, or magical event unless it is a supplemental close-up that does not alter the plot.

## Anatomy and artifact review

At full resolution inspect:

- five-finger structure where visible, believable thumb placement, separated fingertips, natural wrists, and no fused hands;
- clean hair silhouette with no duplicated locks, detached strands, or melted overlap into clothing/background;
- intact eyes, mouths, ears, cheeks, and face outlines;
- sensible layer order where arms, bodies, hair, and props overlap;
- unchanged identity and expression.

## Local correction prompt pattern

For a marked defect, request a localized edit:

“Redraw only the marked hand/hair/face area. Preserve the rest of the image pixel-for-pixel where possible. Reconstruct natural childlike anatomy and a clean silhouette in the same watercolor picture-book style. Remove the annotation mark. Do not add text or change composition, colors, expressions, clothing, background, or aspect ratio.”

If the correction changes more than the intended region, keep the prior image and retry with a tighter instruction.

## Supplemental vertical-comic panels

Supplemental panels may be close-ups of a face, hand, tear, startled animal, doorway, or other existing story beat. Use them sparingly. They must repeat existing characters and events, provide emotional pacing, contain no text, and avoid introducing new plot information.
