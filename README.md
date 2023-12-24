# AGora's SaaS PDF

This is a Demo which contains a SaaS Marketplace with complex user profiles.

## Tecnologies

- [Bun](https://bun.sh/) as the package manager.
- [Next.js](https://nextjs.org/) as the React framework.

## Guide

First of all we init the project executing in our terminal the `npx create-next-app@latest` command:

```console
npx create-next-app@latest agora-saas-marketplace --ts --tailwind --eslint --app --src-dir --use-bun
```

In our case we directly added the name of the project *agora-saas-marketplace* and the following options:

- `--ts`: Initialize as a TypeScript project.
- `--tailwind`:  Initialize with Tailwind CSS config.
- `--eslint`: Initialize with eslint config.
- `--app`: Initialize as an App Router project.
- `--src`:  Initialize inside a `src/` directory.
- ` --use-bun`: Explicitly tell the CLI to bootstrap the application using Bun.

During installation, we will be asked if we want to customize the default import alias (@/*). In which case we will answer `No`.
