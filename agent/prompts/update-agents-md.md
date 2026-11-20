---
description: Summarize this session's work into rules and update the AGENTS.md in the current directory (create if missing)
---
Review the current conversation and extract rules that would have prevented mistakes or
sped up work in future sessions. Update **only** `./AGENTS.md` in the current working
directory. Never touch other AGENTS.md files (parent dirs, global `~/.pi/agent/AGENTS.md`,
or sibling projects).

Steps:
1. Identify concrete rules from this session — project-specific gotchas, tool constraints,
   workflow habits, recurring failure patterns. Only rules backed by something that
   actually happened in this conversation; no generic advice (generic rules belong in the
   global file, which is out of scope here).
2. If `./AGENTS.md` exists, read it first. Merge: keep existing valid rules, add new ones,
   rewrite or drop ones contradicted by what happened this session. Do not delete project
   constraints you cannot verify from the conversation.
3. If `./AGENTS.md` does not exist, create it with a one-line title and the extracted rules.
4. Write each rule as one short line, grouped by topic. Language: match the language the
   user speaks in this session.
5. After merging/writing, do one simplification review pass: re-read the final file,
   merge duplicate or overlapping rules, tighten wording, drop anything redundant —
   target is fewer, shorter rules without losing meaning. Report what was condensed.
6. Report what you added, removed, and why — one line each. If nothing new was worth
   recording, say so instead of padding the file.
