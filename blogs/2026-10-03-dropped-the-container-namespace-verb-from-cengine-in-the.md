---
title: "Dropped the \"container\" namespace verb from $(CENGINE) in the container-* targets so that it will work under Apple Container, which uses the legacy scheme, doubtless to avoid having silly-looking \"container container\" commands. Podman and Docker still support that syntax; it was added to separate these subcommands out, a practice we adopted to make our example commands clear. Broader engine compatibility is more important. Also dropped the \"build buildx\" thing, as that also doesn't work on Apple Container, and it doesn't buy us anything we still need under Docker Engine, as long as you're on 23 or later. Podman never cared. (tags: trunk)"
url: "https://fossil-scm.org/home/info/be50695420d38fd58aba6452f14133a19ccc08646dd139e467a0f073b976a4ee"
date: "2026-10-03"
author: "wyoung"
feed_url: "https://fossil-scm.org/home/timeline.rss"
---
Dropped the "container" namespace verb from $(CENGINE) in the container-* targets so that it will work under Apple Container, which uses the legacy scheme, doubtless to avoid having silly-looking "container container" commands. Podman and Docker still support that syntax; it was added to separate these subcommands out, a practice we adopted to make our example commands clear. Broader engine compatibility is more important.
