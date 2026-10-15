# CHANGELOG — dustinjaeger.net

## 2026-10-15 — word puzzle games reset & timer leak fix
- Fixed Play Again bug across FourInFive, FiveInSix, and SixInSeven where starting a new game could retain previous row inputs or skip to row 2
- Implemented timeout tracking and cancellation (`clearAllGameTimeouts()`) to cleanly abort pending flip/bounce/modal animations upon restart
- Added automatic focus blurring on modal buttons and virtual keyboard keys to prevent physical Enter from re-firing the "Play Again" button while submitting a guess
- Prevented browser default key behaviors on Enter/Backspace and blocked keyboard input while modal backdrop is active
- Added "Reset Statistics" button in the Statistics modal across all three games with confirmation prompt and live zero-reset
- Added URL parameter support (`?reset=all` or `?reset=1`) to conveniently reset player stats via direct link with automatic toast feedback

## 2026-10-14 — word puzzle games upgrade (Option 3 Wordle Engine)
- Transformed FourInFive, FiveInSix, and SixInSeven into feature-complete, modern Wordle clones
- Ergonomic 3-row QWERTY touch keyboard at bottom with real-time key status colors (absent, present, correct)
- Manual Enter submission with two-pass duplicate letter scoring algorithm
- Shake animation and toast alerts for incomplete guesses or words not in dictionary
- Staggered 3D tile-flip reveal animations and victory bounce animation on winning row
- LocalStorage persistence for lifetime stats: games played, win rate, win streak, max streak, and guess distribution bar graph
- Spoiler-free Emoji Share button (📋 Share Result) with automatic clipboard copy
- In-game game switcher pills (4 Letters, 5 Letters, 6 Letters) for quick mode switching
- Modal system for How To Play guide and Game Statistics
- Expanded, clean dictionaries: 902 solutions + 1,546 valid guesses for 4-letter; 1,151 solutions + 3,530 valid guesses for 5-letter; 1,234 solutions + 6,140 valid guesses for 6-letter
- Created safe local backups in `backups/` (FourInFive.html, FiveInSix.html, SixInSeven.html)

- Added live client-side fuzzy search bar across all 80+ tools and software alternatives
- Added interactive category filter pills (Alternatives, Curated, Pentesting, Xbox 360, AI, Emulation, Linux, YouTube)
- Added dynamic results counter and empty state with one-click search reset
- Aligned links page typography and brand color tokens with main portfolio (Space Grotesk, JetBrains Mono, #22d3aa teal accent)
- Updated footer attribution and maintenance date

## 2026-10-14 — navigation & mobile UX overhaul (Phase 2)
- Replaced multi-row wrapped mobile navigation with responsive animated hamburger drawer
- Converted desktop nav to sleek, single horizontal row with left-aligned logo and right-aligned links
- Reorganized nav hierarchy for technical leadership narrative (About → Skills → Experience → Impact → Links → Games → GitHub → Contact)
- Added scroll-margin-top offset to all sections so anchor targets aren't obscured by fixed navbar
- Added branded logo and return link ("← Portfolio") to links-page.html navigation
- Removed stale assistant copy from links-page.html AI section

## 2026-10-14 — site quality & bugfix pass (Phase 1)
- Fixed nav background alpha transparency bug in index.html (added --color-bg-rgb token)
- Fixed timeline dot border syntax typo (border: 3px: 3px)
- Enhanced nav dropdown with semantic button, ARIA attributes, click-outside dismissal, and Escape key navigation
- Added FourInFive to the Games dropdown navigation alongside FiveInSix and SixInSeven
- Sanitized FourInFive word list with clean technology and common vocabulary terms
- Added return navigation link ("← Back to dustinjaeger.net") across FourInFive, FiveInSix, and SixInSeven
- Optimized assets/dragon-icon.png from 309 KB down to 12.6 KB (96% size reduction)
- Added .gitignore for repository hygiene

## 2026-06-26 — index.html redesign (taste-skill)
- Complete visual redesign of index.html using taste-skill principles
- Variable fonts: Space Grotesk (display) + JetBrains Mono (code/data)
- Semantic color tokens (dark mode first, single accent #22d3aa)
- Asymmetric skills grid — featured card spans 2 cols, no more 3 equal cards
- CSS Grid for macro layout, respects prefers-reduced-motion
- 100dvh hero with staggered entrance animations
- Savings badges with distinct green, gradient top-border hover on project cards
- Space Grotesk + JetBrains Mono via Google Fonts (self-hosted in production)

## 2026-06-23 — links-page update
- Added 7 Hermes ecosystem links (Composio skills, Optional Skills Catalog, Creating Skills Guide, Community Projects, Telegram/Slack integrations, Hermes Workspace) to AI & Automation section and rolling 30-day list

## 2026-06-21 — links-page update
- Added Bundled Skills Catalog to AI & Automation section; added to last-30-days list

## 2026-06-20 — links-page update
- Added Awesome Hermes Agent, Agent Skills Standard, and MCP Documentation to AI & Automation section; added to last-30-days list

## 2026-06-18 — links-page update
- Added LobeHub and MCP Servers (Reference) to the AI & Automation section; added both to the rolling last-30-days list

## 2026-06-16 — links-page update
- Added "Last 30 Days — New Links" section to links-page.html for a rolling 30-day FIFO list of recent additions

## 2026-06-16 — nightly maintenance
- Added DistroWatch to the rolling last-30-days links list

## 2026-06-15 — links-page cleanup
- Removed redundant Vimm's Lair card; kept links page structure tidy

## 2026-06-14 — links-page cleanup
- Removed local-build wording from links page
- Added curated links, software alternatives, pentesting/firmware resources, emulation references, and Linux distro links

## 2026-06-13 — homepage polish
- Updated contact email to hermes@dustinjaeger.net
- Removed stale Cloudflare references

## 2026-06-12 — content update
- Replaced placeholder content with real profile data
- Added stats bar and experience timeline