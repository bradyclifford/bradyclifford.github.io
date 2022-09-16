---
layout: post
title: Upcoming entries
published: true
---

Its been awhile since I have journaled my experiences in my profession; 7 years running.

I am rededicating myself to journal atleast once a quarter.  I have experienced many different technologies, patterns, processes, logistics over the past 7 years that I will start to document.

I will probably start on my series of posts regarding my companies team reorganization and Gen2 transition experience:
1. Conway's law and how we decided to reorganize teams and management to align with a verticle instead of horizontal structure.
2. Importance of architecture and strategy decision records
3. Context mapping exercise - company wide (all disciplines) to determine the true boundaries, subdomains, core domains, etc.
4. Method to keep the context map current and accessible to all.  This includes a single place to document our ubiquitous lanages per context.
5. Breaking about a monolith site and database into boundaries, not all at once, little by little
6. Compose micro front-ends into a homogenous site with BFFs and web-components
7. Break down buildtime dependencies between teams by embracing runtime dependencies
8. Implement anti-corruption layers between boundaries (both internal and exterinal)
9. Embrace events over APIs for cross boundary communication
10. No monolith database - embrace the duplicate data across boundaries paradigm - on the bounded context can access directly its database.  All other access must be performed through APIs or events.

Some other experiences I want to eventually document by priority:
1. Finish my Marten usage experience journal entry
2. Importance of a company repo used to start new projects.  Documents architecture decisions.
3. React and how to manage state without complex libraries like Redux - i.e. react-query
4. Zero bug policy
5. Breaking work down in to small, managable, incremental parts
6. Improving the SDLC process and integrating it into automation.
7. Integrating SOC and EDE audit requiremnts into the SDLC process without constricting incremental improvements
8. Shifting left with QA engineers, product managers and UX designers.
9. Story mapping and coming up with a delivary plan while staying agile - focus on milestones / goals, not individual stories and story points
10. GitHub Actions experience - sharing standards functionality with multiple teams and repos
11. Production Support and alerting - integrating with PagerDuty and a public status page site
12. Load and Stress testing experience - k6, kubernetes, reusing Cypres tests and pseudo services for 3rd party integrations
13. CloudEvents, Azure Functions, CosmosDB streams, Azure Event Hub and the Outbox pattern
14. Terraform + Azure experience
15. Integrating a demo environment
16. Integration a failover environment
17. Integrating with a 3rd party both at the API level and UI level - the good, the bad the ugly and how to mitigate risk through contractual tests
18. Distributed tracing with AppInsights & FullStory experience - how to ingegrate multiple AppInsight instances from micro front-ends
19. Home automation experience
