<img src="https://my-badges.github.io/my-badges/fix-4.png" alt="I did 4 sequential fixes." title="I did 4 sequential fixes." width="128">
<strong>I did 4 sequential fixes.</strong>
<br><br>

Commits:

- <a href="https://github.com/dai/ana-lists/commit/565e0a07e41cd8206eb8a130450d2fe4a6bfc395">565e0a0</a>: fix: bookmarklet each star now includes lists array per schema

Each star now has lists:[{githubListId,name,description}] as required
by parseGithubStarsImport validation. Removed unused memberships field.
Moved list context extraction before the repo loop.

Co-Authored-By: Claude Opus 4.6 <noreply@anthropic.com>
- <a href="https://github.com/dai/ana-lists/commit/1c5f3d2a2cbe7c75ac827b3c40bd9bb6b76d05fc">1c5f3d2</a>: fix: bookmarklet sends memberships and removes unused lists field from repos

Previously each repo had a `lists:[]` field and no memberships were sent.
Now builds memberships array to correctly associate repos with the current
list page context. Console log now shows counts for repos/lists/memberships.

Co-Authored-By: Claude Opus 4.6 <noreply@anthropic.com>
- <a href="https://github.com/dai/ana-lists/commit/d7242d8dd6fa652a090a7687b596ebdef24d5722">d7242d8</a>: fix: rewrite buildImportHelper to avoid template literal whitespace issues

Use explicit string concatenation instead of multi-line template literal
to ensure clean one-liner output with correct bracket balancing.

Co-Authored-By: Claude Opus 4.6 <noreply@anthropic.com>
- <a href="https://github.com/dai/ana-lists/commit/da48c5c7374b3984b8da05cd196860ffa2714bae">da48c5c</a>: fix: update bookmarklet DOM selector to match GitHub stars page structure

Use #user-list-repositories h2 a instead of li + a.text-bold.
Description is now extracted from the sibling p element.

Co-Authored-By: Claude Opus 4.6 <noreply@anthropic.com>


Created by <a href="https://github.com/my-badges/my-badges">My Badges</a>