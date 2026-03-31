---
name: Skill Routing Guide
description: One-page reference mapping task type to the correct Claude skill — prevents confusion between overlapping skills
type: reference
---

# HURT! Skill Routing Guide

Use this to pick the right skill immediately. CLAUDE.md always wins; these skills operate within those rules.

---

## Content Creation

| Task | Skill | Notes |
|------|-------|-------|
| Weekly social posts / content calendar | `/hurt-social-manager` | HURT!-specific social engine |
| One-off social post | `/hurt-social-manager` | Same — don't use generic market-social for HURT! |
| Email sequences (copy) | `/market-emails` | B2B partner/employer outreach copy |
| Email HTML template (rendered) | `/email-html-mjml` | Production-ready responsive HTML email — use after copy is approved |
| Ad copy (Google/Meta) | `/market-ads` | Use for paid campaigns |
| Long-form copy (blogs, whitepapers) | `/market-copy` | General copywriting |
| UX/microcopy | `/design:ux-copy` | App and product copy |
| PR pitches, media outreach | `/hurt-pr-strategist` | HURT!-specific; replaces `/market-pr` for HURT! work |
| Client proposal | `/market-proposal` | For external marketing agency clients |
| Presentation / slide deck | `/frontend-slides` | Animated, brand-aligned slide decks |
| Partner newsletter | `/hurt-newsletter-production` | HURT! partner-facing newsletter production |
| Conference prep (speaker brief, booth materials) | `/hurt-conference-prep` | Event and conference preparation workflow |

---

## Brand & Production

| Task | Skill | Notes |
|------|-------|-------|
| Production-ready HTML/visual assets | `/hurt-brand-production` | Final renderable output with brand tokens |
| Brand compliance check on copy | `/brand-voice:enforce-voice` | Run when copy hasn't gone through hurt-social-manager or hurt-brand-production |
| Brand guidelines generation | `/brand-voice:generate-guidelines` | One-time or periodic |
| Stock photography sourcing | `/hurt-stock-sourcing` | Wednesday pipeline; also usable on-demand |
| Figma design implementation | `/figma:figma-implement-design` | Translates Figma to code |

---

## Strategy & Intelligence

| Task | Skill | Notes |
|------|-------|-------|
| Campaign strategy, brief, or CMO-level direction | `/sydneys-cmo-skill` | Sydney's strategic lens |
| Competitive intelligence deep dive | `/market-competitors` | Full competitive analysis |
| SEO audit | `/market-seo` | Content/keyword audit |
| Landing page CRO | `/market-landing` | Conversion rate optimization |
| Marketing audit | `/market-audit` | Full marketing function audit |
| Performance report | `/market-report` | Marketing metrics report |
| YouTube/video research | `/market-youtube` | Competitive and content research |
| Full campaign plan | `/market` | Main orchestrator — delegates to sub-skills |
| Social media audit | `/market-social-audit` | Platform-level audit |

---

## Context & Knowledge

| Task | Skill | Notes |
|------|-------|-------|
| HURT! product facts, approved claims | `/hurt-company-knowledge` | Always invoke as a context layer before generating HURT! copy |
| Finding brand materials across platforms | `/brand-voice:discover-brand` | Discovery across connected MCPs |

---

## System & Ops

| Task | Skill | Notes |
|------|-------|-------|
| Create or modify a skill | `/skill-creator` | Build new automation |
| Update CLAUDE.md | `/claude-md-management:revise-claude-md` | Constitutional updates |
| Schedule a recurring agent | `/schedule` | Cron-based task automation |
| Task management | `/productivity:task-management` | In-session or persistent tasks |

---

---

## MCP Agents (direct tool use — no skill invocation needed)

| Task | MCP | Notes |
|------|-----|-------|
| LinkedIn outreach, profile/company research, job search | LinkedIn MCP | Use directly — search_people, get_person_profile, send_message |
| Read/draft/search Gmail | Gmail MCP | gmail_read_message, gmail_create_draft, gmail_search_messages |
| Schedule meetings, check availability, create events | Google Calendar MCP | gcal_list_events, gcal_create_event, gcal_find_meeting_times |
| CRM lookups, lead/contact/account records | Zoho CRM MCP | ZohoCRM_searchRecords, ZohoCRM_getRecord, ZohoCRM_updateRecord |
| ClickUp tasks, docs, time tracking | ClickUp MCP | See CLAUDE.md Section 6 for ClickUp rules before use |
| Google Drive file search and retrieval | Google Drive MCP | google_drive_search, google_drive_fetch |
| Figma file access, design context | Figma MCP | Use via `/figma:figma-use` skill as prerequisite |

---

## Decision Rules (when in doubt)

1. **Is it HURT! copy?** → Start with `/hurt-company-knowledge` for context, then use the production skill
2. **Social post for HURT!?** → `/hurt-social-manager`, not `/market-social`
3. **PR for HURT!?** → `/hurt-pr-strategist`, not `/market-pr`
4. **Need visual output?** → Add `/hurt-brand-production` after copy is approved
5. **Not sure copy is on-brand?** → Run `/brand-voice:enforce-voice` as a check pass
6. **Strategic campaign question?** → `/sydneys-cmo-skill` first, then delegate to sub-skills
7. **Need a rendered HTML email?** → `/market-emails` for copy → `/email-html-mjml` for production template
8. **Need a deck/presentation?** → `/frontend-slides`
9. **CRM, calendar, LinkedIn, or Gmail task?** → Use the relevant MCP directly — no skill needed
