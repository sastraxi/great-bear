# GREAT ⭑ BEAR
Food delivery sample application metarepo (PostgreSQL / GraphQL / React).

### Outline
* attempt at a fair comparison between Hasura, PostGraphile, and Prisma 
  * why these 3 technologies (why graphql)?
  * why is a food delivery website the best app to build?
  * how is it fair?
  * methodology?
* what are you measuring? 
  * nloc (sql, ts)
  * 
* keep best practices wrt security, frontend tech
  * cookies
  * react hooks - not everything yet
  * styled-components - keeps css near the js, parent-enforces-child-bounds
* postgresql
  * denormalized database - don't prematurely optimise
  * camel_case vs snakeCase
  * auditability
  * security, speed, etc. etc. its a good database mmmmkay?
* aim for the absolute bare minimum of backend boilerplate
* event system
  * hasura: built-in, console helps hugely with debugging
  * postgraphile: pg-pubsub, capture + subscribe to events ourselves
  * prisma:
* developer experience
  * hasura: docker not shutting down cleanly, no js extensibility
  * postgraphile: lots of setup, lots of power. well thought-out APIs.
  * prisma:
* differences in approach
  * hasura: external "appliance", column security + public schema
  * postgraphile: external or library, RLS, different schemas (no col. security)
  * 
* takeaways
  * order of work: hasura, then postgraphile, then prisma
  * 

### Navigation Idea
* first section is the "article", second section is technical detail
* after first section, link to next repo ("next page in the article")
* 

### Repositories
* React + Apollo Frontend: https://github.com/sastraxi/great-bear-frontend
* [Hasura GraphQL Engine](https://github.com/hasura/graphql-engine) backend: https://github.com/sastraxi/great-bear-hasura
* [PostGraphile](https://postgraphile.org) backend: https://github.com/sastraxi/great-bear-postgraphile
* [Prisma](https://www.prisma.io/) backend: https://github.com/sastraxi/great-bear-prisma

The docs in each repository will guide you through setup.

### Tools Used
* VSCode + Plugins
* [GraphQL Playground](https://github.com/prisma/graphql-playground)
* [pgsh](https://github.com/sastraxi/pgsh)
* 
