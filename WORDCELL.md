# WordCell patches

This fork's `wordcell` branch is [storytold/wordcraft](https://github.com/storytold/wordcraft)
`main` plus the small "host mode" changes [WordCell](https://github.com/lennoxmeldrum/wordcell)
needs to show WordCraft as one of its tabs. `main` mirrors upstream unchanged. Each change is its
own commit and is meant to be offered upstream; when upstream has it, drop it here.

| # | Change | Commit subject | Upstream PR |
|---|---|---|---|
| W1 | `WordApp::set_single_window`: draw every document in the host's one window | WordCell host: single-window mode and context reinstall | not yet opened |
| W2 | `WordApp::show_document` is public | WordCell host: public show_document | not yet opened |
| W4 | `panes::headings`: the Navigation pane's heading list, for hosts | WordCell host: panes::headings for hosts' own outlines | not yet opened |
| W5 | `WordApp::reinstall_context`: install WordCraft's fonts, theme and options again | WordCell host: single-window mode and context reinstall | not yet opened |

The plan these come from is `docs/implementation-plan.md` §6 in the WordCell repository.

The upstream workflows in `.github/workflows/` don't run in this fork unless Actions is enabled in
the fork's Actions tab. Leave them off: they need storytold's secrets and shared actions.
