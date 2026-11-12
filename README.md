# DataPulse

DataPulse is a responsive browser-based data engineering workspace built with React, Vite, Tailwind CSS, Lucide React, and Recharts.

## Included workspaces

- **ETL Pipeline:** select ingest, null handling, normalization, deduplication, and one-hot encoding steps; run transformations on the active dataset.
- **Dataset Cleaner:** inspect missing values and duplicate records, impute numeric gaps with mean or median, remove incomplete rows, filter numeric outliers with IQR fences, and export cleaned CSV.
- **Vector Inspector:** explore a sample embedding projection and a clearly labelled similarity-search demonstration.
- **Statistical Studio:** view numeric distributions, mean, median, standard deviation, skewness, and a Pearson correlation matrix.
- **Python Exporter:** generate a starter Pandas or Polars script from the selected transformations and download it.

## Local development

Requires Node.js 20.19+ or 22.12+.

```bash
npm install
npm run dev
```

## Production build

```bash
npm run build
npm run preview
```

## Deploy to Vercel

1. Push or import the `main` branch of [kennedy-blip/datapulse](https://github.com/kennedy-blip/datapulse) in Vercel.
2. Select **Vite** as the framework preset.
3. Use `npm run build` as the build command and `dist` as the output directory.
4. Deploy. No environment variables are required.

The included `vercel.json` already declares the Vite build/output settings and a single-page-app fallback.

## Data and runtime notes

- CSV and JSON uploads are parsed in the browser; the app does not upload datasets to a server.
- ETL transforms and descriptive statistics run locally in the browser.
- The vector collection and semantic-neighbor examples are illustrative demo data, not a connection to a hosted vector database.
- The Python exporter generates a starter script; install the selected Python library and review its input filename and generated columns before running it.
- No backend, API keys, or external database are required for the included demo.
