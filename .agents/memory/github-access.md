---
name: GitHub access checks
description: Verify actual GitHub CLI access instead of relying only on the integration's health status.
---

Check an authenticated GitHub operation before relying on the integration's status. A source-control connection can report active and healthy while the GitHub CLI still requests login. Normal integration connection cards can also reject a source-control connection ID.

**Why:** The integration reported an active OAuth connection, but the publishing CLI had no usable authorization. The normal reconnect and connection forms both rejected the source-control connection ID.

**How to apply:** Use the documented integration recovery flow when authenticated access fails. If its forms reject the source-control connection, report that blockage instead of repeatedly issuing the same card or claiming access is restored. Never read credentials from the environment or ask for raw tokens in chat.
