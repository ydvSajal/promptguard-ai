# PromptGuard AI deliverables

## Feasibility

ChatGPT Sites supports the defensive evaluation prototype as a static app. The original FastAPI/SQLite stack would need separate hosting or a rewrite for the Sites Worker runtime. This build uses browser-local evaluation of supplied evidence and synthetic fixtures. Automated attack generation and live attack execution are outside its scope.

## Prototype

- [x] Read the C23 handover and inventory the workspace.
- [x] Editable baseline and revised prompts.
- [x] Frozen synthetic cases and benign controls.
- [x] Side-by-side raw responses, deterministic evidence and PASS / FAIL / INCONCLUSIVE.
- [x] Compare rates with counts and export the evidence.
- [x] Clearly labeled synthetic fixtures and manual evidence.
- [x] Check JavaScript syntax and run all five scoring and metrics tests with `node --test evaluation.test.mjs`.
- [x] Verify fixture loading, manual response entry, deterministic canary precedence and comparison display in the local browser.
- [ ] Verify the JSON download end to end. The export control is implemented. Browser download permission was declined during verification.
- [x] Deploy privately with Sites. Deployment succeeded and the browser reached the owner sign-in gate. [Open PromptGuard AI](https://promptguard-ai-c23.sajalkumar1765.chatgpt.site).

## Original handover and submission

- [ ] Real OpenAI/Gemini runs and measured provider comparisons. Outside this build.
- [ ] AI attack generator versions, automated target testing, judge and optimizer. Outside this build.
- [ ] Persistent shared run history and server API. Outside this static prototype.
- [x] Document prototype architecture, scoring methodology, demonstration steps and limitations in README.md.
- [x] Draft the C23 technical synopsis and viva notes in C23-synopsis.md.
- [x] Draft the recording script in demo-script.md.
- [ ] GitHub submission repository, final report, demo recording and slides.
- [ ] Verify the original C23 rubric, deadlines and artifact requirements. The guideline PDF was absent from the workspace.



