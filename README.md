# GREAT ⭑ BEAR
Food delivery sample application metarepo (PostgreSQL / GraphQL / React).

### Work-in-progress presentation
* https://docs.google.com/presentation/d/11cpgG0O2LA16ewefyFsgJNcP6aQKR8K9pOURGPAU36s/edit?usp=sharing

### Outline
* attempt at a fair comparison between Hasura, PostGraphile, and Prisma 
  * why these 3 technologies (why graphql)?
  * why is a food delivery website the best app to build?
    * event triggers ("microservices")
    * subscriptions ("push notifications")
  * methodology?
    * stay as close to technology-specific best practices
* what are you measuring? 
  * nloc (sql, ts)
  * 
* keep best practices wrt security, frontend tech
  * cookies
  * react hooks (not everything yet)
  * styled-components - keeps css near the js
* postgresql
  * denormalized database - don't prematurely optimise
  * camel_case vs snakeCase
  * auditability
  * security, speed, etc. etc. its a good database mmmmkay?
* aim for the absolute bare minimum of backend boilerplate
* event system
  * hasura: built-in, console helps hugely with debugging
  * postgraphile: pg-pubsub, capture + subscribe to events ourselves
  * prisma: subscribe via graphql in-app, proxy to consumer-facing graphql api
* developer experience
  * hasura: docker not shutting down cleanly, no js extensibility
  * postgraphile: lots of setup, lots of power. well thought-out APIs.
  * prisma: 
* differences in approach
  * hasura: external "appliance", column security + public schema
  * postgraphile: external or library, RLS, different schemas (no col. security)
  * prisma: exteral "appliance"
* takeaways
  * order of work: hasura, then postgraphile, then prisma
  * 

### Navigation idea
* first section is the "article", second section is technical detail
* after first section, link to next repo ("next page in the article")
* 

### Repositories
* React + Apollo Frontend: https://github.com/sastraxi/great-bear-frontend
* [Hasura GraphQL Engine](https://github.com/hasura/graphql-engine) backend: https://github.com/sastraxi/great-bear-hasura
* [PostGraphile](https://postgraphile.org) backend: https://github.com/sastraxi/great-bear-postgraphile
* [Prisma](https://www.prisma.io/) backend: https://github.com/sastraxi/great-bear-prisma

The docs in each repository will guide you through setup.

### Tools used
* VSCode + Plugins
* [GraphQL Playground](https://github.com/prisma/graphql-playground)
* [pgsh](https://github.com/sastraxi/pgsh)
* 

### What's left to do
* finish the Prisma backend
* refresh on what it's like to work with the three technologies
* build a test harness to run performance / integration tests
* we can use https://www.postgresql.org/docs/11/pgstatstatements.html to get queries / stats
* compare some generated SQL in the presentation
* talk about how this only scratches the surface
