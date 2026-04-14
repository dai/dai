<img src="https://my-badges.github.io/my-badges/fix-5.png" alt="I did 5 sequential fixes." title="I did 5 sequential fixes." width="128">
<strong>I did 5 sequential fixes.</strong>
<br><br>

Commits:

- <a href="https://github.com/dai/o-sumo/commit/16c9b0d27787e7e7d6d3f45d6f61989df2b8d587">16c9b0d</a>: fix: remove unused elapsedDays variable in test

Co-Authored-By: Claude Opus 4.6 <noreply@anthropic.com>
- <a href="https://github.com/dai/o-sumo/commit/5b189fa0766a286a43dd05b29a4852b9174bbba1">5b189fa</a>: fix: resolve test failures from ternary inversions and stale test expectations

- Fix mode ternary in TorikumiDayPage "一覧" link (was swapping result/schedule paths)
- Update TorikumiDayPage sorting test to not depend on specific rikishi names
- Fix torikumi hub page tests for elapsed days and update cadence text
- Fix page test to handle multiple links with same text (current vs past basho)

Co-Authored-By: Claude Opus 4.6 <noreply@anthropic.com>
- <a href="https://github.com/dai/o-sumo/commit/4ce39e4c07c854cf910489d44506a3bed0a3e338">4ce39e4</a>: fix: remove unused useLocation import from TorikumiDayPage

Co-Authored-By: Claude Opus 4.6 <noreply@anthropic.com>
- <a href="https://github.com/dai/o-sumo/commit/85fe12c2a3175cde891eb72d4673910377724c54">85fe12c</a>: fix: route both May and March 2026 archive pages correctly

- Fix parseTopLevelSlug to match 6 or 8 digit dateKeys
- Add explicit path constants: MAY2026_*, MARCH2026_*
- Add March 2026 routes in main.tsx
- Update TorikumiHubPage and TorikumiDayPage to use correct archive based on URL path
- Fix TopLevelSlugPage to redirect to correct archive hub

Co-Authored-By: Claude Opus 4.6 <noreply@anthropic.com>
- <a href="https://github.com/dai/o-sumo/commit/92a55b5903afc303d54e62fab211f9baee8b23e5">92a55b5</a>: fix: route March 2026 archive pages, update homepage past basho section

- Fix findArchiveDay to check MARCH2026_TORIKUMI_DATA for 202603XX dateKeys
- Update homepage to show May 2026 as hero, March 2026 as past basho section
- Add direct links to March 2026 pages: banduke/yotei/torikumi + each day
- Keep all March 2026 /202603-XX pages accessible

Co-Authored-By: Claude Opus 4.6 <noreply@anthropic.com>


Created by <a href="https://github.com/my-badges/my-badges">My Badges</a>