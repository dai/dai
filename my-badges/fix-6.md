<img src="https://my-badges.github.io/my-badges/fix-6.png" alt="I did 6 sequential fixes." title="I did 6 sequential fixes." width="128">
<strong>I did 6 sequential fixes.</strong>
<br><br>

Commits:

- <a href="https://github.com/dai/VinaNihon/commit/9019ececb2125ba10a113b08a6bf5e4b4a7dbe56">9019ece</a>: fix: write proper Vietnamese diacritics in UI copy strings

All Vietnamese UI strings were written without diacritical marks.
Replace with proper Vietnamese orthography using appropriate
diacritics (dấu sắc, huyền, hỏi, ngã, nặng) for each character.

Co-Authored-By: Claude Opus 4.6 <noreply@anthropic.com>
- <a href="https://github.com/dai/VinaNihon/commit/679c89ed15c61096b68736a56dfaf5731be49765">679c89e</a>: fix: add Noto Sans Vietnamese weight 400 for proper diacritics

vietnamese.css only includes weight 300. Body text uses font-weight 400/600
but no Vietnamese 400 was loaded, causing font fallback to miss Vietnamese glyphs.
Add vietnamese-400.css to match regular text weight.

Co-Authored-By: Claude Opus 4.6 <noreply@anthropic.com>
- <a href="https://github.com/dai/VinaNihon/commit/d3373b1436633db252466a2ccc09c486d2b43c79">d3373b1</a>: fix: remove Geist Sans from font stack entirely

Geist Sans has no unicode-range restriction and blocks Noto Sans Vietnamese
from rendering diacritics. Remove Geist Sans from --font-sans so Noto Sans
covers all characters with proper subsets.

Co-Authored-By: Claude Opus 4.6 <noreply@anthropic.com>
- <a href="https://github.com/dai/VinaNihon/commit/79da6756577d9270457666849c4cbecb50ad5982">79da675</a>: fix: use Noto Sans without Geist Sans for Vietnamese UI locale

Geist Sans has no unicode-range restriction so it claims ALL characters,
preventing Noto Sans Vietnamese (with explicit U+1EA0-1EF9 range)
from ever being matched. For html[lang="vi"], use Noto Sans first
so Vietnamese diacritics render correctly.

Co-Authored-By: Claude Opus 4.6 <noreply@anthropic.com>
- <a href="https://github.com/dai/VinaNihon/commit/80f4637f1355cc512938f1711eeef4014e0f7ad4">80f4637</a>: fix: remove html[lang="vi"] font override that broke Vietnamese rendering

Noto Sans JP is Japanese-only and was blocking Vietnamese glyphs.
The vietnamese.css subset already extends Noto Sans with proper diacritics.

Co-Authored-By: Claude Opus 4.6 <noreply@anthropic.com>
- <a href="https://github.com/dai/VinaNihon/commit/29c266a6cfc80338017529c995b2c9edaa009844">29c266a</a>: fix: add Noto Sans Vietnamese subset for proper diacritics rendering

Add @fontsource/noto-sans/vietnamese.css to cover Vietnamese glyphs
(U+1EA0-1EF9) when UI locale is set to Vietnamese.

Co-Authored-By: Claude Opus 4.6 <noreply@anthropic.com>


Created by <a href="https://github.com/my-badges/my-badges">My Badges</a>