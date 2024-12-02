package.json
```json
{
  "name": "configurations",
  "version": "1.0.0",
  "main": "src/index.ts",
  "repository": "git@github.com:abnerpersio/configs.git",
  "author": "Abner Persio <binhopersio@gmail.com>",
  "license": "MIT",
  "scripts": {
    "start": "node dist/index.js",
    "prebuild": "tsc --noEmit",
    "eslint:build": "rimraf dist && esbuild src/index.ts --bundle --platform=node --external:./node_modules/* --outfile=dist/index.js",
    "ts:build": "tsc ."
  },
  "dependencies": {},
  "devDependencies": {
    "@trivago/prettier-plugin-sort-imports": "^3.2.0",
    "@types/node": "^17.0.31",
    "@typescript-eslint/eslint-plugin": "^5.23.0",
    "@typescript-eslint/parser": "^5.23.0",
    "eslint": "^8.15.0",
    "eslint-config-prettier": "^8.5.0",
    "eslint-plugin-import": "^2.26.0",
    "prettier": "^2.6.2",
    "typescript": "^4.6.4"
  }
}
```