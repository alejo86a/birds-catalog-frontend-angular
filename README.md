# CRUD Aves - Frontend

Angular frontend for a simple **CRUD application to manage birds ("aves")**. It lists, creates, edits and deletes bird records, filterable by country/zone, and talks to a REST backend (`crud-aves-backend`) originally hosted on Cloud9 (`https://crud-aves-backend-alejo86a.c9users.io/`).

## What it is

- `AveComponent`: form/view to create or edit a bird (`operacion` input: crear/editar), fetching the list of countries (`PaisesService`) to populate a dropdown.
- `AvesService`: HTTP client wrapping the backend endpoints (`get`, `delete`, `getPorZonas`, `getPorId`, `getPorNombre`).
- `HomeComponent` and a shared `navbar` component for the app shell.
- Generated with Angular CLI (Angular 4.2 / Angular CLI 1.3.2), using Bootstrap 4 (beta), jQuery, Chartist, SweetAlert and bootstrap-notify/switch/table for UI.

## Tech stack

- Angular 4
- Angular CLI 1.3.2
- TypeScript
- Bootstrap 4 (beta), jQuery, Chartist, SweetAlert
- Jasmine/Karma for unit tests, Protractor for e2e

## Running the project

```bash
npm install
npm start      # ng serve, app at http://localhost:4200/
npm test       # unit tests via Karma
npm run e2e    # end-to-end tests via Protractor
```

Note: the app points to a now-likely-defunct Cloud9-hosted backend URL; a working backend (`crud-aves-backend`) is required for data to load.

## Context

Looks like a personal/practice full-stack CRUD exercise (frontend + separate backend repo) built to practice Angular fundamentals (components, services, routing, HTTP) with a simple domain (bird records). Not a production app.
