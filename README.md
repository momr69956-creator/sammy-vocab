# Sammy · Arabic vocabulary

Vocabulary pages with audio for Sammy, one page per lesson, listed on the home page by date
(newest first, grouped by month).

- `index.html`: the home page. Don't edit it by hand: `tools/site.py` writes it.
- `lessons/<date>-<pages>/index.html`: one lesson's vocab page (words, flashcards, quiz,
  speed control).
- `lessons.json`: the list the home page is built from.

To add a lesson:

```
python3 tools/site.py add path/to/built-page.html --date 2026-11-16 --slug pp95-96 --vocab vocab.json
```

Then commit and push. Each lesson keeps its own link, so links already sent to the student keep
working.
