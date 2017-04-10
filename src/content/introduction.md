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
- browser history api by default
- [https://reacttraining.com/react-router/](https://reacttraining.com/react-router/)

---

## Routing Re-cap

- Wrap Routes in BrowserRouter/Router
- Route component takes a `path` and a `component`
- url params in `path` defined with `/:name`
- `match`, `history`, and `location` passed into components
- `Link` component intercepts/avoids reload
- `Switch` component renders first matching route
- `render` function allows 