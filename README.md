# Svelte Practice — Quick Start & Demo

Minimal README with install/run instructions and quick demo steps.

## Prerequisites

- Node.js (v18+ recommended; you have v24+)
- pnpm

## Install

```bash
pnpm install
```

## Development

```bash
pnpm dev
```

Open the URL shown by Vite (usually http://localhost:5173).

## Build (production)

```bash
pnpm build
pnpm preview
```

## Quick demo steps

- Open the app in the browser.
- Counter: click increment/decrement buttons to show reactivity.
- Todo: add a todo (press Enter or click Add), then remove one with the ✕ button.

## Files of interest

- `src/lib/components/Counter.svelte` — counter example (event handling).
- `src/lib/components/Todo.svelte` — todo app (input binding + list).
- `src/routes/+page.svelte` — main page importing the components.

## Screenshot placeholders

- `screenshots/01-home.png`
- `screenshots/02-counter.png`
- `screenshots/03-todo.png`

## Demo notes (speaker bullets)

- Start the server and show the home page.
- Demonstrate the Counter first (quick visible change).
- Demonstrate the Todo: add via keyboard and button, then remove an item.

---

If you want, I can also create the `screenshots/` folder and add a small script to capture the app pages, or produce a single-slide speaker note file. Which next?

# sv

Everything you need to build a Svelte project, powered by [`sv`](https://github.com/sveltejs/cli).

## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```sh
# create a new project
npx sv create my-app
```

To recreate this project with the same configuration:

```sh
# recreate this project
pnpm dlx sv@0.12.5 create --template minimal --types jsdoc --install pnpm Practice
```

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```sh
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

To create a production version of your app:

```sh
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://svelte.dev/docs/kit/adapters) for your target environment.
