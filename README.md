# daily-haiku

Feed for the **Daily Haiku Device** — a CYD (ESP32) display that shows one haiku per day.

`news-haikus.json` holds one entry per day, **newest first**, written each morning by Claude
from the day's most salient world headline (NYT / AP / BBC RSS):

```json
{
  "date": "2026-07-17",
  "haiku": "line one\nline two\nline three",
  "headline": "The headline that prompted it",
  "source": "AP"
}
```

The device fetches the raw file, caches the most recent ~120 days locally, and works
offline from cache. Editorial policy: genuine 5-7-5, image-first, dignity over drama.
