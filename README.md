# AGora's SaaS PDF

This is a Demo which contains a SaaS Marketplace with complex user profiles.

## Tecnologies

- [Bun](https://bun.sh/) as the package manager.
- [Next.js](https://nextjs.org/) as the React framework.
- [shadcn/ui](https://ui.shadcn.com/) as the ui component library.

## Guide

### Step 1 | Installation

First of all we init the project executing in our terminal the `npx create-next-app@latest` command:

> Terminal
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

After the installation, we can preview the result with the following command:

> Terminal
```console
bun run dev
```

<img src="https://raw.githubusercontent.com/Gorachevsky/agora-saas-marketplace/production/media/step_1_default_preview.png" align="center" width="800" height="800" />

### Step 2 | Getting rid of the default code

First of all we will remove the `main` tag and everything it contains inside the `page.tsx` file located in the `src/app` folder. 

We will include a `p` tag with a message "Hello World" to avoid errors and to visualize that everything continues working correctly after having applied the deletion.

Additionally, we will delete the import since it will not be necessary, resulting in the following file:

> src/app/page.tsx
```typescript
export default function Home() {
  return (
    <p>Hello World</p>
  );
}
```

<img src="https://raw.githubusercontent.com/Gorachevsky/agora-saas-marketplace/production/media/step_2_after_clean.png" align="center" width="365" height="251" />

## Step 3 | Implementation of the theme

For this project we will use the ui component library **shadcn/ui** instead of generating them manually: 

> Terminal
```console
npx shadcn-ui@latest init -y
```

After executing the command we will be prompted with a series of questions which we must answer as follows:

```console
Would you like to use Typescript (recommended)? ... Yes
Which style would you like to use? ... Default
Which color would you like to use as base color? ... Slate
Where is your global CSS file? ... src/globals.css
Would you like to use CSS Variables for colors? ... yes
Where is your tailwind.config.js located? ... tailwind.config.ts
Configure the import alias for components: ... @/components
Configure the import alias for utils: ... @/lib/utils
Are you using React Server Components? ... yes
Write configuration to components.json. Proceed? ... yes
```