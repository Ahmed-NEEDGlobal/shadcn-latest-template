# Kolorob-admin

A modern web application built with Next.js, Tailwind CSS, and shadcn/ui —
featuring enforced commit conventions via Commitizen, Commitlint, and Husky.

[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)

---

## Tech Stack

- **Framework:** [Next.js](https://nextjs.org) (latest)
- **Styling:** [Tailwind CSS](https://tailwindcss.com)
- **UI Components:** [shadcn/ui](https://ui.shadcn.com)
- **Package Manager:** [Bun](https://bun.sh)
- **Linting:** [ESLint](https://eslint.org) + [Prettier](https://prettier.io)
- **Commit Conventions:** [Commitizen](https://commitizen.github.io/cz-cli/) +
  [Commitlint](https://commitlint.io) +
  [Husky](https://typicode.github.io/husky)

---

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org) (v18 or later)
- [Bun](https://bun.sh) (latest)

### Installation

1. **Clone the repository:**

```bash
   git clone <your-repo-url>
   cd <your-project-folder>
```

2. **Install dependencies:**

```bash
   bun install
```

3. **Run the development server:**

```bash
   bun dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to see the
result.

You can start editing the page by modifying `app/page.tsx`. The page
auto-updates as you edit the file.

---

## Committing Changes

This project uses **Commitizen** to enforce consistent commit message formatting
based on the [Conventional Commits](https://www.conventionalcommits.org)
standard. Please use the steps below instead of a plain `git commit`.

### Option 1 — Using the npm script (recommended)

```bash
bun run cm
```

### Option 2 — Using `git cz` (requires global install)

Install Commitizen globally if you haven't already:

```bash
npm install -g commitizen
```

Then commit using:

```bash
git cz
```

### How it works

When you run either command, you'll be walked through an interactive prompt:

1. **Select the type of change** (e.g. `feat`, `fix`, `chore`, `docs`)
2. **Enter the scope** (optional — e.g. `auth`, `ui`, `api`)
3. **Write a short description** of the change
4. **Add a longer description** (optional)
5. **Note any breaking changes** (optional)
6. **Reference related issues** (optional)

Husky will automatically lint your final commit message via Commitlint before it
is saved. If your message doesn't follow the convention, the commit will be
rejected with an error.

### Retrying a failed commit

If your commit was interrupted (e.g. a pre-commit hook failed), you can retry
without re-filling the prompts:

```bash
npx cz --retry
```

### Commit types reference

| Type       | Description                                     |
| ---------- | ----------------------------------------------- |
| `feat`     | A new feature                                   |
| `fix`      | A bug fix                                       |
| `docs`     | Documentation changes only                      |
| `style`    | Formatting, missing semicolons, etc. (no logic) |
| `refactor` | Code change that is neither a fix nor a feature |
| `test`     | Adding or updating tests                        |
| `chore`    | Build process, tooling, or dependency updates   |

---

## Scripts

| Command      | Description                            |
| ------------ | -------------------------------------- |
| `bun dev`    | Start the development server           |
| `bun build`  | Build the app for production           |
| `bun start`  | Start the production server            |
| `bun lint`   | Run ESLint                             |
| `bun run cm` | Start an interactive Commitizen commit |

---

## Learn More

- [Next.js Documentation](https://nextjs.org/docs)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [shadcn/ui Documentation](https://ui.shadcn.com)
- [Conventional Commits Specification](https://www.conventionalcommits.org)
- [Commitizen GitHub](https://github.com/commitizen/cz-cli)

---

## Deployment

The easiest way to deploy this app is via the
[Vercel Platform](https://vercel.com/new). Check out the
[Next.js deployment docs](https://nextjs.org/docs/app/building-your-application/deploying)
for more details.
