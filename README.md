## Development

- Install node & yarn (volta)

```bash
volta install node
volta install yarn
```

- Install dependencies

```bash
yarn
yarn dev
```

## Libraries

- Basic

```bash
yarn add -D @types/node @types/react @types/react-dom prettier eslint-config-prettier eslint-plugin-react-hooks @next/eslint-plugin-next
```

- UI

```bash
yarn add react-icons lucide-react
npx shadcn@latest init -d
```

## Configuration

### ESLint

- write your rules in `eslint.config.mjs` (if you want)

### VSCode

- write below in `.vscode/settings.json`

```json
{
  "npm.packageManager": "yarn",
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.formatOnSave": true,
  "editor.formatOnPaste": true,
  "editor.codeActionsOnSave": {
    "source.addMissingImports": "explicit"
  },
  "javascript.preferences.importModuleSpecifier": "non-relative",
  "typescript.preferences.importModuleSpecifier": "non-relative"
}
```

### Environment Variables

- copy `.env.sample` to `.env.local` and fill in the values

## Deploy

- add GAS_URL as secret in GitHub Actions
