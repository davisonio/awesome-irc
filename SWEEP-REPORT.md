# Sweep Report

## Summary

This is an awesome-list (Markdown only, no buildable code), so steps 1-5 were replaced by a dead-link and formatting sweep plus a link-check GitHub Action.
I fixed 5 dead or moved links and 15 formatting issues, and moved the link check from awesome_bot (EOL Ruby 2.7) to a separate lychee job.

## Done

- **Dead-link sweep: done.** Checked all 174 unique URLs. Fixed:
  - Textual: `codeux.com/textual` now redirects to `textualapp.com`.
  - gamja and Goguma: the sr.ht pages say both projects moved to Codeberg (`git.sr.ht` returned 502). Goguma now links to its homepage `goguma.im`.
  - #Ubuntu: the Ubuntu wiki was rebuilt and the `IRC/ChannelList` and `IRC/Guidelines` pages are gone (404). The entry now points to the official Ubuntu community support docs (which cover the IRC channels) and the Ubuntu Code of Conduct.
  - contributing.md: `help.github.com/pull-requests` (404) now points to `docs.github.com/en/pull-requests`.
- **Formatting sweep: done.** Removed spaces inside link URLs (Twitch Plays, netsplit.de) and a trailing slash (RobustIRC). Closed an unbalanced parenthesis (Quassel). Fixed capitalisation (IRCCloud, ZNC) and the typo "managenent". Normalised `Javascript` to `JavaScript` and the trailing periods on bridge entries. Fixed the garbled Modern IRC Documents description, renamed `img2src` to `img2irc` to match its repo, and added a final newline to contributing.md.
- **Link-check GitHub Action: done.** `.github/workflows/main.yml` now has two jobs:
  - `awesome_lint`: runs awesome-lint on Node 22.
  - `link_check`: runs lychee (`lycheeverse/lychee-action@v2`) with retries, configured in the new `lychee.toml`, which keeps the existing awesome.re and davison.io allowlist. It runs on push or PR to master, weekly on a schedule, and on manual dispatch.
  - The only token used is the built-in `GITHUB_TOKEN`, to avoid github.com rate limits. No configured secrets are needed. Workflow permissions are now `contents: read`.
- 1. Maintenance: skipped. There are no dependencies or build.
- 2. Tests + CI: skipped (no code to test). CI was updated as described above.
- 3. Security: skipped. Nothing handles auth, user data or untrusted input.
- 4. Site audit: skipped. This is not a website; GitHub renders the README.
- 5. Grind: skipped. There is no TypeScript and no Workers config.

## Test coverage

There are no tests (0 before, 0 after): no code. The equivalent checks are awesome-lint and the link check.

## Commands verified passing

- `npx awesome-lint readme.md`: all rules pass except `awesome-github`, which needs the GitHub API. This sandbox's proxy blocks the API, so that rule fails here. It passes in CI.
- `lychee --config lychee.toml readme.md contributing.md` (with github.com excluded locally): 107 OK, 0 errors.
- `git ls-remote <url> HEAD` succeeded for every `github.com/<owner>/<repo>` link in the list. github.com web pages return 403 through this sandbox's proxy, so this was the only way to check them here.

## Follow-ups needing a human

- The new workflow runs only on master and on PRs to master, so it has not run yet. Opening a PR from this branch will exercise both jobs.
- `lychee.toml` excludes four hosts that block automated clients but load fine in a browser: `bitchx.sourceforge.net` (Cloudflare challenge), `packages.debian.org` and `salsa.debian.org` (anti-bot challenge), and `davison.io` (cert hostname mismatch). Spot-check them occasionally.
- Fix the `davison.io` TLS certificate so it can be removed from the allowlist.
- Two entries have no description: `node-irc` and `IRC-BF`. I did not add copy.
- Several listed projects are likely unmaintained (for example lazybot, skyweb2irc and Skybot). Their links still resolve, so I kept them. Removing them is a curation call.
- Some statistics in the list may be out of date ("Searches 563 different networks", "318 different networks").
