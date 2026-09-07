---
name: write-in-pencil
description: Generate an exploratory brainstorming image that looks like a designer's pencil sketch on paper and communicates both an idea and the thinking around it. Use when a user's task would benefit from a hand-drawn visual for exploring and discussing ideas.
---

# Write in Pencil

- Generate an image as if a designer had sketched it on paper with a pencil.
- This is a deliverable for brainstorming and exploration. Express the idea together with its intent and traces of exploration so viewers can understand the content and the considerations behind it.
- Use an available image generation tool or skill (such as `$imagegen`).

## Roles

- **The request-handling AI develops the proposal and its design intent.**
  - Follow the [Design Guidelines](references/design.md) to develop the proposal and select the drawings, explanations, and notes to include.
  - Pass the selected content to the image generation model, identifying the parts it concerns, and provide background and constraints separately.
  - Attach the full [Image Generation Guidelines](references/image-generation.md) verbatim, without interpreting or summarizing them.
- **The image generation model develops the concrete proposal and how to communicate it visually.**
  - Develop the supplied design further.
  - Represent the supplied content while preserving its meaning. Decide its wording, composition, placement, and balance of drawings and text.
  - Generate the image according to the Image Generation Guidelines.
