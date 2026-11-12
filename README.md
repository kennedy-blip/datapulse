# DataPulse

A responsive data engineering workspace for building ETL workflows, cleaning datasets, exploring vector embeddings, running descriptive analytics, and exporting Python scripts.

## Stack
- React + Vite
- Tailwind CSS
- Lucide React
- Recharts

## Local development
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
Import `kennedy-blip/datapulse` in Vercel. Framework preset: Vite. Build command: `npm run build`. Output directory: `dist`. No environment variables are required for the local demo features.

> Data processing runs in the browser using the uploaded dataset. The vector inspector and pipeline execution are local demonstrations; they do not claim to connect to a remote vector database or Python runtime.
