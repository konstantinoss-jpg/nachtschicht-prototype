# Nachtschicht frontend prototype

An independent, interactive frontend design for Nachtschicht. All moderation data and actions are simulated. This repository does not modify or connect to the original Twitch moderator project.

## Preview

Private hosted preview: https://nachtschicht-design.gentlecamel16.chatgpt.site

To run locally, open `index.html` in a modern browser, or serve this folder:

```sh
python3 -m http.server 8080
```

Then visit http://localhost:8080. No dependency installation or build is required. Fonts load from Google Fonts, with system-font fallbacks.

## Features

- Responsive moderation dashboard and simulated chat feed
- Custom message testing with deterministic sample rules
- Shadow/live simulation, permission ceilings, pause and resume
- Review queue with undo
- Searchable, filtered, paginated activity and CSV export
- Title proposal approval, dismissal, and restoration
- Browser-local persistent state, settings, and demo reset

Moderation level and permissions affect new simulated decisions. Language, house rules, and community expressions are saved preferences; an AI model is not connected. No Twitch credentials or backend are included.

## Validation

JavaScript syntax and interaction logic were checked, including pause/resume, permissions, confirmations, review undo, settings persistence, filtering, pagination, CSV export, escaped chat content, and reset. Visual browser QA has not been completed.

## Branch

The frontend is maintained on `prototype/nachtschicht-frontend`; `main` retains the initial repository README.
