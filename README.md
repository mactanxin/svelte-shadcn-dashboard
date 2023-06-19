# A demo dashboard using `SvelteKit`, `TailwindCSS` and amazing-`shadcn-ui` port of [`sveltekit/shadcn`](https://www.shadcn-svelte.com/docs/installation).

## Installing

## New Project

<Steps>

### Create a new project

Use the SvelteKit CLI to create a new project.

```bash
npm create svelte@latest my-app
```

### Add TailwindCSS

Use the `svelte-add` CLI to add Tailwind CSS to your project.

```bash
npx svelte-add@latest tailwindcss
```

### Run the CLI

```bash
npx shadcn-svelte init
```

This will install dependencies, update your TailwindCSS configuration, add the `$components` path alias to your `svelte.config.js` file, and configure the `cn` utils for you.

</Steps>

## Manual Installation

<Steps>

### Add Tailwind

Use the `svelte-add` CLI to add Tailwind CSS to your project.

```bash
npx svelte-add@latest tailwindcss
```

### Add dependencies

Add the following dependencies to your project:

```bash
npm install tailwindcss-animate class-variance-authority clsx tailwind-merge lucide-svelte
```

### Path Aliases

Use the `$components` alias to make it easier to import your components. This is how you can configure the `$components` alias in `svelte.config.js`:

```js title="svelte.config.js" {7-8}
/** @type {import('@sveltejs/kit').Config} */
const config = {
  // ...
  kit: {
    // ..
    alias: {
      $components: "src/lib/components",
      "$components/*": "src/lib/components/*"
    }
  }
};
```


# create-svelte

Everything you need to build a Svelte project, powered by [`create-svelte`](https://github.com/sveltejs/kit/tree/master/packages/create-svelte).

## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```bash
# create a new project in the current directory
npm create svelte@latest

# create a new project in my-app
npm create svelte@latest my-app
```

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

To create a production version of your app:

```bash
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://kit.svelte.dev/docs/adapters) for your target environment.
