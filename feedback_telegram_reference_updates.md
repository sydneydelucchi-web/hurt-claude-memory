---
name: Telegram reference message updates
description: Regenerate and send Telegram pinned reference messages after significant Claude ecosystem changes
type: feedback
---

After any significant update to Sydney's Claude ecosystem, regenerate and resend the relevant Telegram reference message(s) so she can update her pinned messages.

**Why:** She pins reference cards in the Telegram bot chat for quick mobile access. Stale pins are worse than no pins.

**How to apply:** After completing work that changes any of the following, resend the affected message via the Telegram Bot API (token + chat ID are in ~/telegram-bot/.env):

- **Resend the quick reference card** (keyword routing) when:
  - New keywords or routes added to routes.yaml
  - New scheduled tasks created
  - Existing agent names changed

- **Resend the project directory card** when:
  - A new project directory is created
  - A project is significantly repurposed or renamed
  - New Desktop scripts are added
  - New report output file patterns are introduced

Use the same formatting style (HTML parse_mode, bold headers, arrow separators). Send to chat_id 8688417915 using the bot token in ~/telegram-bot/.env.
