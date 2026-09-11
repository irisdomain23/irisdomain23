<p align="center">
  <img src="https://raw.githubusercontent.com/irisdomain23/irisdomain23/main/assets/header.svg" alt="Iris Lin — Front-End Engineer · Accessibility" width="880"/>
</p>
<p align="center">
  <img src="https://raw.githubusercontent.com/irisdomain23/irisdomain23/main/assets/now.svg" alt="now" width="720"/>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB" height="22"/>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/CSS-1572B6?style=flat&logo=css&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/WCAG_2.2-0052CC?style=flat&logo=w3c&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/Vite-646CFF?style=flat&logo=vite&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/Vitest-6E9F18?style=flat&logo=vitest&logoColor=white" height="22"/>
</p>

---

Front-end engineer in Singapore. I build design systems, and most of my time goes to the parts that get skipped — focus order, empty states, and what a component does when the data never arrives.

## What I work on

Component APIs, design tokens, docs, and the migration work that comes after. A fair share of my week is spent reading someone else's markup and deciding whether the fix belongs in the component or in the page that misused it.

## Stack

Every day:

- **React + TypeScript** — hooks, `strict` on, generics only when they earn their keep
- **CSS** — custom properties, cascade layers, container queries; I reach for CSS before JS
- **Vite + Vitest + Testing Library** — queries by role, never by test id if a role exists

Regularly:

- **Storybook** as the review surface, not the documentation of last resort
- **Figma tokens → CSS custom properties**, generated rather than hand-copied
- **Playwright** for the handful of flows that would cost money if they broke
- **Node** for build tooling, and nothing more ambitious than that

## Accessibility, specifically

- WCAG 2.2 AA is the floor for anything I ship, not a phase at the end
- axe-core in CI catches the boring 40%; the rest needs a keyboard and a screen reader
- VoiceOver on Safari and NVDA on Firefox, because they disagree and both users exist
- Focus is a design decision — where it lands after a dialog closes belongs in the spec
- Reduced motion, forced colours, and 200% zoom are test cases, not edge cases

## Selected projects

### [iris-ui](https://github.com/irisdomain23/iris-ui)

A small React + TypeScript component library — Button, Tag, Tooltip — with no runtime
dependencies and keyboard behaviour written before the styling.

### [a11y-checklist](https://github.com/irisdomain23/a11y-checklist)

A single-file accessibility checklist that runs offline in a browser tab. Built to hand to
designers and PMs who are not going to install anything.

### [css-snippets](https://github.com/irisdomain23/css-snippets)

Layout, gradient, and dark-mode snippets I got tired of re-deriving, kept in one place with
notes on when each one breaks.

### [react-hooks-lib](https://github.com/irisdomain23/react-hooks-lib)

Three hooks I use across every project — `useDebounce`, `useLocalStorage`, `useMediaQuery`.
Typed, dependency-free, small enough to read in one sitting. The ones I copy into a new
codebase before the first component is written.

### [focus-trap-util](https://github.com/irisdomain23/focus-trap-util)

A focus trap for dialogs and overlays — Tab and Shift+Tab cycle within the container's
focusable elements, focus moves to the first element on mount, and the cleanup function
restores normal tab order when the overlay closes. If a role exists in the DOM, it should
be reachable by keyboard.

## How I work

- Read the spec before the blog post. MDN and the WCAG *Understanding* pages settle most arguments.
- A component that needs a wrapper `div` to be usable is not finished.
- `aria-*` is what you reach for when semantic HTML runs out, not where you start.
- If a design has no defined focus, error, and empty state, the design is not done — I will ask
  before I build it, not after.
- Ship the boring version, then measure. Most performance work is deleting something.

## Currently

- Moving a component library's overlay layer onto the Popover API and CSS anchor positioning,
  with a fallback path for browsers that are not there yet
- Working through the success criteria that landed in WCAG 2.2 — target size and focus
  appearance are the ones changing our components the most

## 📊 Activity

<p align="center">
  <img height="160" src="https://gh-profile-stats.zli39uclan.workers.dev/stats?username=irisdomain23&accent=61dafb&cell=circle&hide_border=true"/>
  <img height="160" src="https://gh-profile-stats.zli39uclan.workers.dev/top-langs?username=irisdomain23&accent=61dafb&cell=circle&hide_border=true"/>
</p>
<p align="center">
  <img width="720" src="https://gh-profile-stats.zli39uclan.workers.dev/activity?username=irisdomain23&accent=61dafb&cell=circle&hide_border=true"/>
</p>

## Contact

Issues and discussions on any of the repos above. That is the fastest way to reach me, and I
read all of them.

---

Singapore · UTC+8 · [github.com/irisdomain23](https://github.com/irisdomain23)
