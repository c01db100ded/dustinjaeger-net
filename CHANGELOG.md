# CHANGELOG — dustinjaeger.net

## 2026-10-14 — links page upgrade (Phase 3)
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