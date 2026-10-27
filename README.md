# React Module Federation: Host and Remote Demo

A small example of a host application loading a component exposed by a separate remote application using Webpack Module Federation.

## Project structure

- `app1` — host application
- `app2` — standalone remote application exposing a `Button` component

## Run locally

Install dependencies using the package manager and lockfile maintained by this repository. Then run from the repository root:

```bash
yarn install
yarn start
```

The documented development setup serves the host on port 3001 and the remote on port 3002.

- Host: [http://localhost:3001](http://localhost:3001)
- Remote: [http://localhost:3002](http://localhost:3002)

## What to inspect

- Remote component exposure and host consumption
- Local development server configuration
- How the remote URL is configured for the host

## Limitations

This is a basic one-way example, not a complete micro-frontend platform. Before deployment, define remote versioning, failure/loading behavior, shared dependency compatibility, origin/CORS rules, and a deployment strategy for independently released applications.
