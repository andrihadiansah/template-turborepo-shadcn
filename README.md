# Turborepo Template With Shadcn UI

This Turborepo Template is created by [my self](https://github.com/andrihadiansah/)

## Requirements

- Text Editor (i recommend vscode)
- NodeJS >=18 or later, for installation [NodeJS](https://nodejs.org)
- pnpm 9.x.x or later, as `Package Manager` installation [pnpm](https://pnpm.io/) with command:

```sh
npm install -g pnpm@latest-10
```

-

## Using this example

Run the following command:

```sh
git clone https://github.com/andrihadiansah/template-turborepo-shadcn
```

```sh
pnpm i
```

```sh
turbo dev
```

## Checking Update

To check your package dependency use command

```sh
pnpm outdated

```

then use

```sh
--filter=web
```

to filter your folder selected like `web` in apps, `ui` in packages folder.

After know the selected package.json some dependency are outdated, we can update select the dependency with command for example:

```sh
pnpm update react-dom
```

or all dependency with command:

```sh
pnpm update --latest
```

## What's inside?

This Turborepo includes the following packages/apps:

### Apps

- `web`: a [Next.js](https://nextjs.org/) app, you can add more apps.

### Packages

- `@workspace/eslint-config`: `eslint` configurations (includes `eslint-config-next` and `eslint-config-prettier`)
- `@workspace/typescript-config`: `tsconfig.json`s used throughout the monorepo

- `@workspace/ui`: - a reusable React UI library powered by ShadCN and Tailwind v4, maintained for shared use in `web` and other workspace apps

Each package/app is 100% [TypeScript](https://www.typescriptlang.org/).

### Utilities

This Turborepo has some additional tools already setup for you:

- [TypeScript](https://www.typescriptlang.org/) for static type checking
- [ESLint](https://eslint.org/) for code linting
- [Prettier](https://prettier.io) for code formatting
- [TailwindcssV4](https://tailwindcss.com) for styling
- [ShadcnUI](https://ui.shadcn.com/docs) for UI library

### Remote Caching

> [!TIP]
> Vercel Remote Cache is free for all plans. Get started today at [vercel.com](https://vercel.com/signup?/signup?utm_source=remote-cache-sdk&utm_campaign=free_remote_cache).

Turborepo can use a technique known as [Remote Caching](https://turborepo.com/docs/core-concepts/remote-caching) to share cache artifacts across machines, enabling you to share build caches with your team and CI/CD pipelines.

By default, Turborepo will cache locally. To enable Remote Caching you will need an account with Vercel. If you don't have an account you can [create one](https://vercel.com/signup?utm_source=turborepo-examples), then enter the following commands:

```sh
cd your-turborepo
```

#### With [global `turbo`](https://turborepo.com/docs/getting-started/installation#global-installation) installed (recommended)

```sh
turbo login
```

##### Without [global `turbo`](https://turborepo.com/docs/getting-started/installation#global-installation), use your package manager

```sh
npx turbo login
yarn exec turbo login
pnpm exec turbo login

```

This will authenticate the Turborepo CLI with your [Vercel account](https://vercel.com/docs/concepts/personal-accounts/overview).

Next, you can link your Turborepo to your Remote Cache by running the following command from the root of your Turborepo:

#### With [global `turbo`](https://turborepo.com/docs/getting-started/installation#global-installation) installed (recommended)

```sh
turbo link
```

##### Without [global `turbo`](https://turborepo.com/docs/getting-started/installation#global-installation), use your package manager

```sh
npx turbo link
yarn exec turbo link
pnpm exec turbo link

```

## Useful Links

Learn more about the power of Turborepo:

- [Tasks](https://turborepo.com/docs/crafting-your-repository/running-tasks)
- [Caching](https://turborepo.com/docs/crafting-your-repository/caching)
- [Remote Caching](https://turborepo.com/docs/core-concepts/remote-caching)
- [Filtering](https://turborepo.com/docs/crafting-your-repository/running-tasks#using-filters)
- [Configuration Options](https://turborepo.com/docs/reference/configuration)
- [CLI Usage](https://turborepo.com/docs/reference/command-line-reference)
