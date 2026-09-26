# notes

field notes, rough drafts, and braindumps from harman kajla.

this repository serves as an obsidian vault on phone and laptop, and feeds directly into [h4rman.com/notes](https://h4rman.com/notes).

---

## how to write a note

### 1. frontmatter structure
every note must include frontmatter at the top:

```markdown
---
title: "your note title"
description: "optional 1-sentence hook or summary"
date: "2026-09-26"
tags: ["jee", "thoughts"]
published: true
---

write your raw content here.
```

### 2. publishing rule
- **`published: true`**: the note will be built, rendered, and indexed on [h4rman.com/notes](https://h4rman.com/notes).
- **`published: false`** (or omitted): the note stays a private draft in your vault. it will never be built or shown on the website.

### 3. using the template
a starter template is located at `template.md` (and `templates/note-template.md`). in obsidian, configure core plugin **templates** to point to the `templates` directory, or just copy `template.md`.

---

## syncing & workflow

### on laptop
open this folder (`~/notes`) as a vault in obsidian. write your note, flip `published: true` when ready, then commit and push:
```bash
git commit -am "note: title" && git push
```

### on mobile
clone this repository into your mobile git client (or use the obsidian git community plugin). write on the go, flip `published: true`, and sync.
