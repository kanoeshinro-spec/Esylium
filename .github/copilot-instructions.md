# Repository instructions for GitHub Copilot

- Work on the existing project and imported prototype; do not create an independently generated replacement application or game engine.
- Before making changes, read `README.md`, `docs/CURRENT_STATE.md`, and `docs/ARCHITECTURE.md`.
- Follow conventions and tools established by the actual codebase. Do not invent build, test, or deployment commands.
- Prefer small, reviewable changes and report what was actually tested.
- Keep game rules separate from UI and AI-generated output. Validate critical actions and state changes deterministically.
- Add tests for new critical mechanics using the project's existing test infrastructure.
- Preserve existing saved games and data formats where possible; document necessary migration or compatibility changes.
- Do not give the client unchecked authority over critical game state.
- Keep credentials, API keys, and other sensitive data out of the repository. Use examples without real credentials where configuration is needed.
- Document relevant architecture decisions and distinguish implemented behavior from proposals.
- Keep Esylium and Game: Creation technically independent. Do not copy code or add a dependency without explicit authorization.
- Do not perform broad architecture rewrites unless specifically requested and justified by the existing code.
- Use only game content for which the project has appropriate rights.
