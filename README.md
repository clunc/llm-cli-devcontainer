# llm-cli-devcontainer
VS Code devcontainer template with Node 20, pnpm, Git, GitHub CLI, Codex CLI, Claude CLI, and extensions preinstalled. Copy `.devcontainer/` into a repo, adjust ports/postCreate/postAttach commands, reopen in container, and start coding with LLM CLIs ready. Ports include 1455 for Codex auth.

## Adding to another repo (squashed)

From the target repo root, pull just the `.devcontainer/` folder and commit as one change:

```bash
rm -rf .devcontainer && \
git fetch https://github.com/clunc/llm-cli-devcontainer.git main && \
git checkout FETCH_HEAD -- .devcontainer && \
git commit -am "Add devcontainer template (squash)"
```

After copying, tweak `devcontainer.json` ports/postCreate/postAttach commands as your project needs.
