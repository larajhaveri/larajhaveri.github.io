---
name: Ruby bundle isolation
description: Diagnose successful bundle installation followed by missing-gem errors in an isolated local bundle.
---

When `bundle install` succeeds but `bundle exec` still reports missing gems, check the configured bundle path instead of changing dependency versions.

**Why:** Bundler reported using globally available HTTP gems without installing them into its isolated local path. Runtime execution then could not find those gems. Installing the existing locked versions into the configured bundle path restored the Jekyll build without changing the lockfile.

**How to apply:** Inspect `bundle config list` and read the current lockfile for required versions. Ensure missing gems are physically installed in that configured path. Keep local dependency files ignored, and distinguish these environment errors from site-code failures.
