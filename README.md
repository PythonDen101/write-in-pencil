# Write in Pencil

An AI agent skill for exploring ideas through pencil-on-paper sketches.

This is the skill featured in [this post on X](https://x.com/momotarabitch/status/2094962393025806638).

[こちらの投稿で紹介したスキルです。](https://x.com/momotarabitch/status/2094962393025806638)

Use it for product UI concepts, single-slide ideas, and diagrams that explain relationships or how something works. The sketch includes the proposal and useful notes about its intent and alternatives.

Main drawings use monochrome graphite. Blue and orange annotations add emphasis. Results are exploratory raster images, not finished UI, editable slides, or exact-text documents.

## Requirements

An agent that can read Markdown-based skills and access an image-generation tool. This repository provides instructions only: it does not include an image model, API credentials, an image-generation service, or an installer. Availability, cost, data handling, and output quality depend on the agent and provider you use.

## Install

Clone or download this repository, review its files, then place the `write-in-pencil` folder in the skills directory supported by your agent. Keep `SKILL.md`, `references/`, and `agents/` together.

```sh
git clone https://github.com/momotarabitch2/write-in-pencil.git
```

If your agent does not support skill discovery, ask it to read `SKILL.md` and the linked guidelines before generating an image. The `agents/openai.yaml` file is optional UI metadata for compatible hosts. The design instructions are not tied to one agent vendor.

## Usage

```text
Use write-in-pencil to sketch an app where friends save places they want
to visit together, discuss the options, and decide when to go.
```

```text
Use write-in-pencil to create a one-slide concept explaining how a team
records work observations, reuses them, and adds results to the original notes.
```

日本語でも依頼できます。

```text
write-in-pencilで、仕事の気づきを同僚が使い、結果を元の記録に追記する
仕組みを説明する、1枚スライドの構想を描いてください。
```

The request-handling agent develops the proposal and selects its content. The image-generation model develops the visual expression while preserving that meaning. See [SKILL.md](SKILL.md) for the full workflow.

## Privacy and safety

- Prompts and reference images may be sent to your configured image-generation provider. Share only content you are authorized to send and check that provider's data policies.
- Remove credentials, personal information, confidential business details, and private screenshots before requesting a sketch.
- This repository contains no executable scripts, automatic installers, dependencies, telemetry, or GitHub Actions workflows. Your agent and its tools still operate under their own permissions.
- Review downloaded instructions before use. For repeatable use, pin a commit you have reviewed and review later updates before adopting them.
- Inspect generated images for inaccurate claims, text errors, and unintended sensitive content before sharing.

## License

[MIT](LICENSE). The license covers this repository's files. Use of image-generation services and generated outputs is subject to the relevant provider terms and any third-party rights.
