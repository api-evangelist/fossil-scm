---
title: "Allow building on Windows under the MINGW64 shell. Multiple changes needed: * pacman command in the build doc was performing a search, not a \"sync\", what other package systems call install; thus, no-op * configure was presuming presence of /dev/null meant \"not MinGW\"; doubtless there are MinGW setups where this is the case, but the modern MinGW64 terminal is not one of these * the guards against trying to use linenoise on Windows weren't triggered for this type of build, causing link failures (tags: trunk)"
url: "https://fossil-scm.org/home/info/ddba8ea2432c734b0a2287caec4246c6423b1cdf71049b72bb4aea04e67de946"
date: "2026-10-05"
author: "wyoung"
feed_url: "https://fossil-scm.org/home/timeline.rss"
---
Allow building on Windows under the MINGW64 shell. Multiple changes needed: * pacman command in the build doc was performing a search, not a "sync", what other package systems call install; thus, no-op * configure was presuming presence of /dev/null meant "not MinGW"; doubtless there are MinGW setups where this is the case, but the modern MinGW64 terminal is not one of these * the guards against trying to use linenoise on Windows weren't triggered for this type of build, causing link failures (tags: trunk)
