
# OpenPecha's technology stack

## Frontend

- [Typescript](https://www.typescriptlang.org/) for Javascript
- [TailwindCSS](https://tailwindcss.com/) for CSS
- [React](https://reactjs.org/) for frontend builds
- [Metabase](https://www.metabase.com/) for reporting and dashboards

> **Note**: When feasible, follow the client-side rendering pattern.

## Backend

- [Hasura](https://hasura.io/) for application APIs 
- [AdonisJS](https://adonisjs.com/), or [NestJS](https://nestjs.com/) for cases when [Hasura](https://hasura.io/) is insufficient
- [psql](https://www.postgresql.org/) for relational datastores
- [TerminusDB](https://terminusdb.com/) for graph/connected datastores
- [FastAPI](https://fastapi.tiangolo.com/) for routing
- [Auth0](https://auth0.com/) for access management

## Monitoring and analytics

- [MixPanel](https://mixpanel.com/) for application analytics
- [Sentry](https://sentry.io/welcome/) for application error and performance monitoring
- [Smartlook](https://www.smartlook.com/) for application user behavior analytics
- [Prometheus](https://prometheus.io/) for log file analysis

## DevOps and workflow
 
- Centralize CI/CD and related processes and assets on GitHub
- Run frontends on Cloudflare Pages
- Use Cloudflare edge workers whenever it makes sense
- Run everything else on bare-metal, except when very small compute units are sufficient, in which case use cloud instances 
- Virtualize cloud instances and bare-metal with Docker
- Use Poetry for Python projects
- Use [Postman](https://www.postman.com/) for API docs
- Run everything that can't run on Cloudflare Pages, as Docker containers
- Build Docker images in CI/CD and deploy to GitHub image repository, where it is then pulled onto the server
- When new servers are deployed, the setup of that server is as-code
 

> **Note**: 
> - Tenzin [suggested](https://github.com/OpenPecha/Housekeeping/issues/7) [Django](https://www.djangoproject.com) instead of AdonisJS/NestJS.
> - Elie suggested using [Recoil](https://recoiljs.org) for React states.