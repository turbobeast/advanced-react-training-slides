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
- Routing (with React Router V4)
- Server-Side Rendering (with express.js)
- Lazy Loading

---

## Get Started

```bash
git clone git@github.com:turbobeast/advanced-react-training.git
cd advanced-react-training
npm install
```

---

## Routing

- Navigation within a single-page application (without page reload)
- Deep-link (address-bar)
- Browser History

---

## React Router V4

- Declarative API
- Browser history API by default
- Docs: [https://reacttraining.com/react-router/](https://reacttraining.com/react-router/)

---

## Routing Re-cap

- Wrap Routes in BrowserRouter/Router
- Route component takes a `path` and a `component`
- URL params in `path` defined with `/:name`
- `match`, `history`, and `location` passed into components
- `Link` component intercepts/avoids reload
- `Switch` component renders first matching route
- `render` function allows more control over what is rendered

---

## Server-Side Rendering

- What is SSR?
- Pros/Cons
- High-level implementation overview

+++

## What is SSR?
- Server-Side Rendering
- AKA Universal, Isomorphic
- initial DOM and state are generated and served

+++

## Pros/Cons

- Pros
  - Fast initial load
    - cached DOM content and state
    - reduces client requests on load
  - SEO
- Cons
  - Additional code to manage (server.js/index.js)
  - Two mindsets while coding (client/server)

+++

## High-level implementation overview
1. Statically build
- Serve content using express
- Add custom routes for landing pages
- Update index.html to have replaceable content
- Read index.html as a string
- Import and initialize the store
- Setup babel and import root of code (index.js)
- Render to a string using initialized store
- Inject DOM and state into markup
- Serve up cached markup on request

+++

## Live coding exercise

Code along or just watch
- Clone the repo: `git clone git@github.com:turbobeast/advanced-react-training.git`
- Change directory: `cd advanced-react-training`
- Install dependencies: `npm install`

---

## SSR Re-cap
- Setup express server to serve up static content from build
- Add custom routing for landing pages
  - generate DOM content
  - generate initial state
  - serve cached content

---

## Lazy Loading

- Break-up initial bundle
- Site loads faster
- Less JS to parse/compile (faster TTI)

---

## Lazy Loading Re-cap

- `require.ensure()` tells webpack to split bundle
- Path in `require()` must be hard-coded
- Higher-order component handles calling load function and re-rendering `setState`
- Object rest spread transform `{...props}`

---

# Thanks