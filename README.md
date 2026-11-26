# learn_claude

A learning log for getting comfortable with Claude Code. Entries are in date order, and new entries go at the bottom.

---

## Ideas to learn next
- [ ] Write a `CLAUDE.md` with project instructions (`/init`)
- [x] Make a git commit with Claude
- [ ] Try plan mode (`Shift+Tab`) before a bigger change
- [ ] Use `/help` and explore slash commands
- [ ] Set permissions so Claude asks less often (`/permissions`)
- [ ] Build a small script or app in this repo

---

## Template for new entries

Copy this to the bottom of the log for each new session:

```markdown
## YYYY-MM-DD

### Topic
- What I asked / tried:
- What I learned:
- Commands or shortcuts worth remembering:
```

---

# Log

## 2026-11-26

### Opening links from the terminal (Mac)
- **iTerm2, Ghostty, Warp, VS Code terminal:** `Cmd` + click the URL.
- **Terminal.app:** `Cmd` + double-click, or right-click → **Open URL**.
- **Any terminal:** type `! open https://example.com` in Claude Code. The `!` prefix runs a shell command directly.
- Or just ask Claude: "open https://example.com in my browser".

### Running Claude Code "at root"
- **As the root user (`sudo claude`):** works, but risky. Every command runs with full admin rights, `--dangerously-skip-permissions` is blocked as root, and `~/.claude` files can end up owned by root.
  - Instead: run as your normal user and let Claude ask before `sudo` for specific commands.
- **In the root folder (`cd / && claude`):** works, but Claude sees the whole disk as the project, which makes it slow and noisy.
  - Instead: start in your project folder. Use `/add-dir` or full paths for files elsewhere.

### Editing files with Claude
- Asked Claude to edit this README. It looked at the file first, then asked what to change.
- Lesson: say *what* you want changed for faster results.
- Set the README up as a learning log, then rearranged it so new entries go at the bottom.
