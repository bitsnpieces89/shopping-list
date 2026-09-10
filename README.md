Two gotchas:

1. **Changing the app later.** Edit `index.html` on GitHub, but also bump `CACHE = 'shoplist-v1'` in `sw.js` to `v2`, `v3`, and so on. That string is what tells phones the cached copy is stale. Skip it and your changes silently won't appear.
2. **Your data lives in that browser under that exact URL.** Rename the repo and the list is gone from the app's point of view — still on the phone, but under the old address. Clearing browsing data wipes it too. If it ever becomes precious, the easy insurance is an export button that dumps the list as text.
