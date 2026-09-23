# Composition and lettering specification

## Shared principles

- Compose with existing pixels. Use deterministic raster layout for scaling, cropping, masks, borders, and text.
- Do not use image generation to recreate the full page or long image.
- Apply high-quality resampling and preserve color; avoid repeated resizing or recompression.
- Add text last so the text remains sharp and editable during layout iteration.
- Prefer regular-weight Chinese fonts with smooth antialiasing such as ClearTypeGridFit.

## Black-text optimized grid page

### Layout

- Pure white outer background.
- Header uses direct crops of the original date, title, and author.
- Follow the source's reading order and approximate grid proportions.
- Use straight black, pen-like borders with consistent visual weight.
- Artwork must meet the inside of the border with no white seam. Slightly enlarge or crop a panel when necessary.
- Do not crop away an important head, hand, protagonist, animal, action, or prop merely to fill a cell.

### Typography

- Narration: black, regular KaiTi-style Chinese type, slightly larger.
- Character speech: black, regular SimSun/Song-style Chinese type, slightly smaller.
- Avoid bold text unless the source explicitly demands it.
- Match the source's approximate placement while improving legibility.
- If a nearby light area is available, move text slightly into it and omit the background.
- Over dark or busy art, use a tight white translucent backing with generous transparency. Keep the backing only a little larger than the text and never let it cover or cross a black border.
- Verify punctuation, names, repetitions, and unusual phrases against the source rather than silently normalizing them.

## Vertical comic long image

### Canvas and pacing

- Default to roughly 900 px width and a content-driven height suitable for previewing and reading on a phone.
- Use a white background and deliberate breathing room. The page need not be tightly packed.
- Mix full-width panels, paired panels, insets, and occasional diagonal cuts. Use diagonals only where they clarify motion or emotion.
- Occasional artwork may break across a frame, but preserve a clear reading order.
- Preserve full scenes when possible; do not overcrop the first panel or reduce a story-critical subject such as a crow to a fragment.

### Narration

- Use black, regular KaiTi-style type, larger than dialogue.
- Place narration in natural negative space or in a tight translucent white box when the art is busy.
- Do not cover faces, key actions, dialogue, animals, or borders.

### Dialogue bubbles

- Use black, regular SimSun/Song-style type, smaller than narration.
- Ordinary speech uses a clean white oval or gently organic bubble with a black outline and **no tail**.
- Strong emotion may use a white spiky bubble with a black outline and slightly larger regular Song-style type.
- Avoid long pointers and detached divider lines.
- Place bubbles in negative space, at a panel edge, or straddling a white gutter when needed. Never cover a face, protagonist, story-critical subject, or narration.
- When a bubble and character feel crowded, expand the surrounding white space or reposition the bubble before shrinking the character.

## Final inspection checklist

- Correct panel order and continuous story.
- Latest corrected art used in both outputs.
- No accidental white seams inside grid cells.
- Header is a source crop, not a redraw.
- Narration and dialogue use the correct font classes and sizes.
- Ordinary bubbles have no tails; spiky bubbles are reserved for strong emotion.
- No text, bubble, or translucent backing overlaps a face, key subject, narration, or black border.
- Text is pure black, smooth, correctly punctuated, and readable at preview scale.
- Full-resolution PNG and lightweight preview both open successfully.
