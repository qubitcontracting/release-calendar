# release-calendar

Auto-generated iCal feeds, refreshed nightly at 04:17 America/Edmonton.

Replaces the FirstShowing.net "FS Release Schedule" Google Calendar, which stopped
being updated on 2025-08-11.

## Subscribe

| Feed | Contents | Raw URL |
|---|---|---|
| `movies.ics` | Popular theatrical releases | `https://raw.githubusercontent.com/qubitcontracting/release-calendar/main/movies.ics` |
| `tv.ics` | TV season premieres | `https://raw.githubusercontent.com/qubitcontracting/release-calendar/main/tv.ics` |
| `all.ics` | Both combined | `https://raw.githubusercontent.com/qubitcontracting/release-calendar/main/all.ics` |

Google Calendar: **Other calendars → + → From URL** → paste a raw URL above.

## Sources

- **Movies** — [TMDB](https://www.themoviedb.org/) `/discover/movie`, theatrical release
  types, popularity >= 5, 180-day window.
- **TV** — [TVmaze](https://www.tvmaze.com/api) `/schedule`, episode 1 only (= season
  premiere, covers both new series and returning seasons), show weight >= 80,
  types: Scripted / Animation / Documentary.

TVmaze needs no API key. Data thins out beyond ~4 months, so the TV horizon is
naturally shorter than the movie horizon.

Generator lives on the Docker LXC at `/opt/release-cal/`.
