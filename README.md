# Coach Scorecard — front end

Static front end for an internal dashboard. **This repository contains no data.**

The page renders a Google sign-in prompt and then reads its figures at runtime
from a private Google Sheet, using the viewer's own credentials. Access is
controlled by that Sheet's sharing, enforced by Google — not by anything in this
repository. A visitor who is not one of the named accounts sees an explanatory
message and no figures.

This repo is public only because GitHub Pages requires it. Everything of
substance — the data, the process, and the generator that produces this file —
lives in a separate private repository.

## Contents

| File | |
|---|---|
| `index.html` | Generated. Do not edit here; it is built from the private repo. |
| `.nojekyll` | Skips Jekyll processing |

## Configuration

The OAuth client ID embedded in the page is public by design; it is restricted by
its authorized JavaScript origins. The spreadsheet ID is likewise not a secret —
reading it requires being granted access to the Sheet.
