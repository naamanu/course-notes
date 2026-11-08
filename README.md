# Course notes index

A one-page, week-by-week index of public university course materials, grouped
by school and then by course. Each course shows its offerings side by side.
The page only links to the originals; no course content is copied.

## Build locally

```sh
python3 build.py          # writes _site/index.html (standard library only)
open _site/index.html
```

## Add a course

Edit `courses.json`. Schools contain courses, and courses contain offerings:

```json
{
  "id": "uw",
  "name": "University of Washington",
  "courses": [{
    "id": "uw-cse452",
    "code": "CSE 452",
    "title": "Distributed Systems",
    "offerings": [{
      "label": "Spring 2025",
      "parser": "uw-createcal",
      "calendar": "https://courses.cs.washington.edu/courses/cse452/25sp/calendar/calendar.html",
      "home": "https://courses.cs.washington.edu/courses/cse452/25sp/"
    }]
  }]
}
```

- `id` must be unique; it's used for page anchors and the summaries file name.
- `parser` picks how to read the calendar. `uw-createcal` handles UW CSE
  course calendars. Other schools' sites will need a new parser: write a
  function in `build.py` that returns the lecture list described above
  `PARSERS`, then register it there.
- `dirs` (optional) lists directory listings to scan for files the calendar
  doesn't link. The regex's first group is the week number.

If one offering fails to load, the build still succeeds and the page shows an
error for that offering.

## Add your own notes

Put short summaries in `summaries/<course-id>.json`, keyed by week number:

```json
{ "3": "Paxos: proposers, acceptors, why a majority quorum makes it safe." }
```

Summaries show at the top of that week and are included in search.

## Deploy

Push to `main` on GitHub, then go to **Settings → Pages** and set **Source** to
**GitHub Actions**. The workflow rebuilds on every push, every Wednesday, and
whenever you run it from the Actions tab.
