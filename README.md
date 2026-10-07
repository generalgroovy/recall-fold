# Recall Fold

Turn your own passage into a gentle, self-rated recall exercise, one hidden word at a time.

Serve this folder with `python -m http.server 8000`, then open http://localhost:8000. No install, account or runtime dependency is required.

Choose **Fold a word**, recall it, and **Reveal word**. **Remembered** removes that occurrence from the session; **Again** puts it at the end. **Choose words** lets you select the exact occurrences to practice. **Use your text** replaces the passage and suggests up to four long words; these are simple lexical suggestions, not semantic analysis. A short passage uses its first words instead. End practice always returns to the passage. **Undo text replacement** restores the previous passage and chosen words after either text replacement action; it starts no active round.

Text and chosen occurrences save locally. Reload starts a fresh session. Saving failure does not block practice; keep the original text elsewhere. Input is plain text, limited to 20,000 characters. This app does not evaluate comprehension, infer learning, upload text, or provide spaced repetition between visits. Every button is keyboard accessible.

Run `npm test` or `node --test`. Tests cover occurrence identity, selection validation, queue behavior, completion and malformed storage.

Original implementation inspired by the passage-focused simplicity of GeneralGroovy's Webreader. It turns reading into active recall rather than duplicating speech playback.

Potential depth, not shipped: phrase spans, portable study sets, optional contextual hints, and reviewed long-term practice scheduling.
