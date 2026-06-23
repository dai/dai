<img src="https://my-badges.github.io/my-badges/chore-commit.png" alt="I did a little housekeeping! 🧹" title="I did a little housekeeping! 🧹" width="128">
<strong>I did a little housekeeping! 🧹</strong>
<br><br>

Commits:

- <a href="https://github.com/dai/VinaNihon/commit/dbb6b32814f99ece7237e46945fbdae0aaff45c5">dbb6b32</a>: chore(deps): bump dependencies to latest stable

- wrangler ^4.74.0 -> ^4.103.0
- astro ^6.0.5 -> ^6.4.8
- @astrojs/cloudflare ^13.1.2 -> ^13.7.0
- @astrojs/check ^0.9.8 -> ^0.9.9
- tailwindcss / @tailwindcss/vite ^4.2.1 -> ^4.3.1
- @fontsource/geist-mono ^5.2.7 -> ^5.2.8
- @fontsource/noto-sans ^5.2.7 -> ^5.2.10

TypeScript is held at ^5.9.3: the 6.x line merged lib.dom.iterable
into lib.dom, which collides with the SpeechRecognitionEvent /
SpeechRecognitionErrorEvent declarations in src/scripts/translator.ts.
Re-evaluate when those globals are removed.

Verified: npm run check (0 errors), npm run build, astro dev (HTTP 200).


Created by <a href="https://github.com/my-badges/my-badges">My Badges</a>