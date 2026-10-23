---
title: "Update src/sha1hard.c to match the current upstream implementation, which LLM analysis assures us is faster. The only local changes applied were minor formatting, add 'static' to a few functions, and remove those which fail the resulting 'defined but not used' warning. This change requires stdint.h: C99 but unsupported by MSC until mid-2000-teens, so this might not build with an ancient MSC. Passes tests with rebuild, test-integrity, and this check-in. (tags: trunk)"
url: "https://fossil-scm.org/home/info/d243deba6a63cf4e2b0c58fe153505153dbdf26df75b2647b0d01ad511d88efe"
date: "2026-10-16"
author: "stephan"
feed_url: "https://fossil-scm.org/home/timeline.rss"
---
Update src/sha1hard.c to match the current upstream implementation, which LLM analysis assures us is faster. The only local changes applied were minor formatting, add 'static' to a few functions, and remove those which fail the resulting 'defined but not used' warning. This change requires stdint.h: C99 but unsupported by MSC until mid-2000-teens, so this might not build with an ancient MSC.
