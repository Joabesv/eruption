# Eruption 🌋

> Next Generation Boilerplate for React/Typescript, built on top of Vite ⚡️

_It's fast! Even the tests are fast, thanks to Vite with Vitest ⚡️_

# What's in the boilerplate

- Vite
- React
- Typescript
- Vitest
- Testing Library
- Dev Tools
  - ESLint
  - Prettier
  - CommitLint
  - Husky
  - Lint-Staged

# Installation

This project uses DEGIT to scaffold.

first, clone the project and give it a name

```Bash
npx degit github:devmozao/eruption#main your-project-name
```

then, to start the project

```Bash
cd your-project-name
npm install
npm run dev
```

## Try it online

Want to try Eruption without clone local? Try it on [StackBlitz](https://stackblitz.com/fork/github/devMozao/eruption)

# Commits

This project have commits configured to follow the Conventional Commits's best practice.

To commit, you must follow the convention `<type>[optional scope]: <description>`. In practice, it would be as follow:

```git
git commit -m "feat: add button component"

```

Then, Husky will start the pre-commit hook and run lint-staged, who will run `prettier` and `lint` to validate code format and code lint. If you fail to follow any one of these validations above, the commit will be aborted.

After that, if everything is validated correctly, Husky will proceed with the commit-msg hook, where he will evaluate if your commit message is following the Conventional Commit's best practice and will run the tests of your project. If any of the tests are broken, the commit will be aborted. You must fix the tests before proceeding.

As a best practice, it is strongly suggested that you avoid skip validations. If you need to change the way your commit messages are written, just go to file `commitlint.config.ts` and you will find there the configs needed.

# Motivation

Everything started because I was in need of a good, solid, reliable and fast boilerplate to work with React/Typescript projects. I was working with Create-React-App and Webpack but both of them wasn't that good at all, specially in performance. Later on I discovered that I could use Vite to replace Webpack, so here we are now. =)

I believe that Eruption as it is right now, is an excellent starting point to any React/Typescript project, with enough dev tools to help you to write the best software possible and ship to production without any headaches.

# License

MIT
