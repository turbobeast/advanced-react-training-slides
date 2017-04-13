# React Training - Part 3

# Rangle.io

>Presented by:

>Michael Faust - @turbobeast

>Rob Brander - @rbrander

---

## Prerequisites

- Access to the command line
- Node.js (v6 or higher)
- NPM (v3 or higher)
- Code editor (Sublime, Atom, etc.)
- Some JavaScript knowledge (ES5/ES6)
- Basic React Knowledge (Part 1 of this course)
- Basic Redux Knowledge (Part 2 of this course)

---

## Structure of this Training

- 2 hours training
- 20 min Intro/Slides
- 1h 40 min Live Coding

---

## Curriculum

- Routing (with React Router V4)
- Server-Side Rendering (with express.js)
- TBD

---

## Routing

- Navigation within a single-page application (without page reload)
- Deep-link (address-bar)
- Browser history

---

## React Router V4

- declarative API
- browser history API by default
- Docs: [https://reacttraining.com/react-router/](https://reacttraining.com/react-router/)

---

## Routing Re-cap

- Wrap Routes in BrowserRouter/Router
- Route component takes a `path` and a `component`
- url params in `path` defined with `/:name`
- `match`, `history`, and `location` passed into components
- `Link` component intercepts/avoids reload
- `Switch` component renders first matching route
- `render` function allows more control over what is rendered

---

## Server-Side Rendering

- improves SEO (pages can be indexed/read by crawlers and bots)
- accessibility (app works without javascript enabled)
- performance

---

## SSR Re-cap

---

## Lazy Loading

- break-up initial bundle
- site loads faster
- less JS to parse/compile (faster TTI)

---

## Lazy Loading Re-cap

- `require.ensure()` tells webpack to split bundle
-  path in `require()` must be hard-coded
- higher-order component handles calling load function and rendering
- object rest spread transform `{...props}`

---

# Thanks