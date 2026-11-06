# NW Link Validator

Runs a Playwright-based link validation against URLs listed in a CSV file.

## Local run

```bash
npm ci
npx playwright install chromium
npm run link-validate -- --unified --file url-temp.csv
```

## GitHub Actions

Workflow file: `.github/workflows/link-validator.yml`

- Run it from GitHub: **Actions → Link Validator → Run workflow**
- Outputs are uploaded as an artifact named `link-validator-reports`.