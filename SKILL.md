---
name: academic-mentor-portrait
description: Generate or refine formal academic mentor and faculty portraits from a reference image. Use when a user asks for a professional teacher, professor, scholar, or academic headshot with preserved identity, business attire, studio lighting, polished pose, or a neutral studio background.
---

# Academic Mentor Portrait

Create a photorealistic academic-professional portrait with the supplied image as an identity reference. Use the `imagegen` skill and built-in image generation/editing tool.

## Default visual brief

- Preserve recognizable face, natural complexion, hairstyle, and expression from the reference.
- Use a black business blazer and crisp white shirt unless the user specifies different clothing.
- Use a frontal medium portrait, centered, with shoulders and torso nearly square to the camera.
- Default pose: arms naturally crossed at chest level; relaxed, anatomically correct hands; direct eye contact; gentle, confident smile.
- Use a perfectly smooth deep charcoal-gray studio gradient with no texture, props, text, logos, or watermark.
- Rebuild lighting rather than copying the reference: soft, even studio key and fill, natural luminous skin, gentle face-and-body modeling, soft shadows, and no harsh contrast.
- Render as premium, photorealistic professional photography with detailed but natural retouching.

## Workflow

1. Treat the supplied portrait as an identity reference, not a style reference. State the identity-preservation constraint clearly in the prompt.
2. For a new portrait, use the `identity-preserve` image-generation workflow. For a revision to the latest generated image, use the latest image as the edit target and change only the requested attribute.
3. Keep the prompt structured: subject identity, clothing, pose, composition, backdrop, lighting, constraints.
4. For pose edits, explicitly preserve face, hairstyle, clothing, expression, framing, lighting, and background. Request correct fingers and relaxed hands.
5. Inspect the result for a square-to-camera torso, symmetric shoulders where requested, realistic hands, identity fidelity, and an even dark-gray background. If needed, iterate with one targeted adjustment.

## Prompt core

Use this concise base specification, adapting only user-requested details:

```text
Use case: identity-preserve
Asset type: formal academic faculty portrait
Input image: identity reference
Primary request: Create a photorealistic professional portrait of the same adult woman. Preserve recognizable facial features, hairstyle, natural complexion, and business attire. Frontal centered medium portrait, with torso and shoulders nearly square to the camera, direct eye contact, and a gentle confident smile. Arms naturally crossed at chest level, with relaxed anatomically correct hands.
Scene/backdrop: perfectly smooth deep charcoal-gray gradient studio background, no props or texture.
Lighting/mood: fully regenerated soft, even studio lighting; luminous natural skin; gentle dimensional modeling; soft shadows; no harsh contrast.
Constraints: preserve identity; no added accessories, text, logo, watermark, extra fingers, distorted hands, busy background, or exaggerated retouching.
```
