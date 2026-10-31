# Dreamina feature investigation

## What REA captured

REA ran a controlled browser capture at <https://dreamina.capcut.com/ai-tool/home?createTab=chat> in a provider-owned Chromium session. The session started with empty cookies, local storage, and session storage. REA captured the page's accessibility tree and screenshot.

- Evidence ID: `ev_efe01af6f95e845c04a52c49f6b18e9b9feaf4d33319168c3f95eff0f32b96f9`
- Browser: Chromium 156.0.4314.58
- Observed page elements: AI Agent tab; prompt field; Upload references; Auto; Skills; Generate; prompt suggestion chips; More skills.
- In the initial empty-prompt state, Generate was disabled.

The supplied reference screenshot also shows the AI Agent composer, Auto and Skills controls, and suggestion chips.

## What Dreamina documents

Dreamina's [AI Agent and Canvas feature page](https://dreamina.capcut.com/ai-video/ai-agent) says Canvas search can locate nodes by **name, text, or type**. It also describes using labels, groups, thumbnails, and previews to find assets and ongoing work. The page describes moving AI Agent outputs into Canvas for organization and refinement.

These search capabilities are **documented**, not dynamically observed in the REA capture. The capture stayed on the initial Create screen; it did not open a populated Canvas. Search ranking, exact-match behavior, case handling, filters, and empty-state behavior remain unknown.

## How the prototype applies the evidence

The updated [REA Evidence Workspace](dreamina-evidence-workspace.html) adapts those ideas to REA's evidence-centered workflow: target-scoped investigation prompts, searchable evidence by title/text/type, and separate labels for observed, documented, and inferred claims. Its sample data comes from the capture and linked official documentation. The prompt action is a local prototype; it does not connect to a live REA session or an AI model.

Project context: [REA repository](https://github.com/lumenmarketingc-ux/rea) and its [website design guide](https://github.com/lumenmarketingc-ux/rea/blob/main/website/style-guide.md).

