---
name: Retiring generated artifacts
description: How to remove an unwanted generated artifact and its managed workflows when changing project structure.
---

Artifact-owned workflows cannot be removed through the ordinary workflow-removal callback. Stop them before retiring an unwanted artifact directory; removing that directory also removes the platform's artifact registration and managed workflows.

**Why:** The platform rejected direct removal of managed workflows. After the approved scaffold directories were deleted, it automatically removed the corresponding artifact registrations and workflows.

**How to apply:** Use this only when the user has approved retiring an artifact or replacing its scaffold. Confirm the directory contains no user work that needs preservation before deleting it.
