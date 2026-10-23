---
"@nanocollective/nanocoder": patch
---

`web_search` now escapes result titles and snippets before passing them to the model. Newlines are collapsed and markdown characters such as `=`, `[`, `|` and `<` are backslash-escaped, so a search result can no longer add headings, links or extra lines to the tool output. URLs keep only `http` and `https` schemes and are shown as `<url>` with whitespace removed.
