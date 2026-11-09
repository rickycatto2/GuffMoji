---
name: guffmoji
description: Turn a supplied avatar, Bitmoji, cartoon, or portrait into a reusable black-and-white satirical comic character, then create reaction images, expression sheets, and slapstick scenes. Use when the user asks for GuffMoji or this kind of reference-based caricature; not for generic photo edits or unrelated illustrations.
metadata:
  version: "0.1.0"
---

# GuffMoji

Create recognizable characters with the frantic energy of mid-century satirical magazine cartoons: black ink, elastic expressions, absurd physical comedy, and hand-lettered noise.

Image generation requires a tool that accepts reference images. Text-only environments can prepare prompts and character profiles.

## Choose the task

Infer the mode from the request; the user does not need to type a command.

| Mode | Use when | Default output |
| --- | --- | --- |
| CREATE | Converting a new avatar, portrait, or cartoon | One character sheet with a neutral full-body pose and three expressive poses |
| REACT | Showing one feeling or response | One readable reaction image |
| SCENE | Illustrating an event, interaction, or gag | One comic panel with a clear visual punchline |
| SHEET | Expanding an established character | One sheet of the requested expressions or poses |

Honor requested panel counts, dimensions, captions, and style changes over these defaults.

## Ground the character

Inspect the supplied image before composing the generation prompt. Identify the visible anchors that distinguish this character: face shape, hair, glasses, facial hair, headwear, outfit, shoes, jewelry, and silhouette. Preserve those anchors while stretching expressions and movement. Do not give every character the same nose, face, or body.

For CREATE, use the source image as the reference. If clothing or lower-body details are not visible, use a simple compatible design and identify it as a design choice rather than an observed fact. Establish a readable baseline pose so later images have a useful reference.

For REACT, SCENE, and SHEET, prefer the user's latest approved character sheet and corrections. Use a written profile as supplementary guidance. When a new request intentionally changes an outfit or feature, apply that change without treating it as an error.

If no character reference is available and the request depends on a specific likeness, ask for it. Do not claim to remember or access a sheet from another chat. If the user wants an invented character, proceed from their description.

Ricky and Ellie are demonstration characters, not universal defaults. Use their supplied sheets only when the user requests them. In multi-character scenes, bind each name to its own reference and keep hair, accessories, proportions, and wardrobe distinct.

## Visual grammar

- Use black ink on white paper. Build tone with crosshatching, stippling, and solid blacks rather than gray gradients, color washes, or glossy rendering.
- Combine a readable silhouette with lively, uneven pen lines. Keep faces, hands, and the central action legible even when surrounding details become frantic.
- Exaggerate mouth shapes, body language, thin expressive fingers, flailing limbs, bending joints, and oversized footwear as appropriate to the character. Preserve the identifying features.
- Make humor situational: a sleeve caught in a printer, a chair escaping at the wrong moment, an absurdly expanding pile of revisions. Give motion a cause and a visible consequence.
- Use sweat drops, vibrating contours, debris, and action lines where they clarify the gag. Leave breathing room around the focal action.
- Add short, irregular, hand-lettered sound effects when they help: “PAF!”, “GRONK!”, “SPLORT!”, “CREEEAAAK!” Respect requests for no text. Keep requested dialogue concise and legible.
- Do not add an artist's signature, brand logo, or watermark. Do not present generated work as an original drawing by a named artist.

## Generate and check

Use the available image-generation tool, supplying the actual reference images along with the character anchors, scene action, composition, and lettering instructions. Follow the host's image-tool workflow. Generate the requested image directly when tools and inputs are available.

If image generation is unavailable, clearly say so and provide a ready-to-use prompt that identifies which reference images to attach. Never describe an ungenerated image as completed.

Inspect the result when the environment permits. Check that the character is recognizable, separate characters have not exchanged features, the main action reads clearly, and the requested lettering and panel count are present. Correct material failures using the reference sheet and a focused edit when supported. Report any unresolved limitation without promising perfect consistency.

Present the image with minimal commentary. For CREATE, suggest saving the approved sheet for reuse. When the user asks for a portable character record, use [the character-profile template](references/character-profile.md). Do not imply that profiles or images are automatically saved across chats.
