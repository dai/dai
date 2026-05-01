<img src="https://my-badges.github.io/my-badges/fix-2.png" alt="I did 2 sequential fixes." title="I did 2 sequential fixes." width="128">
<strong>I did 2 sequential fixes.</strong>
<br><br>

Commits:

- <a href="https://github.com/dai/VinaNihon/commit/b0ec239f42ddee95683cd0a80829814344d0e5f9">b0ec239</a>: fix: use Web Share API for LINE button to share translation text

Previously used window.open() with LINE social plugin URL which caused
iOS Safari to share the page URL instead of the translation text.
Now uses navigator.share() for native share sheet with proper text sharing.

Co-Authored-By: Claude Opus 4.6 <noreply@anthropic.com>
- <a href="https://github.com/dai/VinaNihon/commit/ccf4a0f669ee4e8f1b5e91534f900ec51f336af5">ccf4a0f</a>: fix: use closest() for locale toggle click and add flag icons

- Replace globe SVG icons with Japan and Vietnam flag icons for locale toggle
- Fix locale toggle click handler using closest() to properly handle SVG child elements
- Add debug console.log that was left in applyLocale (removed)

Co-Authored-By: Claude Opus 4.6 <noreply@anthropic.com>


Created by <a href="https://github.com/my-badges/my-badges">My Badges</a>