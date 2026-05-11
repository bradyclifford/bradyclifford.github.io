---
title: Merging Two Operating Models After an Acquisition
date: 2026-05-08
tags:
  - architecture
  - operating-models
  - mergers
  - conways-law
  - agile
excerpt: When companies merge, the biggest challenge is often not technology integration. It is the collision between operating models.
published: "true"
---

One of the most difficult transformations I have experienced was not a cloud migration, a monolith decomposition, or a platform modernization effort.

It was attempting to merge two fundamentally different operating models after an acquisition.

[![Conway's Law Diagram](images/posts/2026-04-25-Merging-Two-Operating-Models.png)](/images/posts/2026-04-25-Merging-Two-Operating-Models.png)

Most organizations assume the challenge will primarily be:

* Systems integration
* Tooling consolidation
* Vendor rationalization
* Data migration
* Identity integration

In reality, those are usually secondary problems.

The real challenge is organizational.

**Specifically:**
How two groups think about ownership, delivery, governance, architecture, and accountability.

---

# The Mistake Most Organizations Make

The most common failure pattern I have seen is leadership attempting to standardize too quickly.

Typically this includes:

* Forcing common tooling
* Forcing common workflows
* Forcing shared governance models
* Centralizing delivery processes
* Unifying team structures
* Enforcing identical SDLC practices

The assumption is:
“If everyone operates the same way, integration becomes easier.”

In practice, the opposite often occurs.

Instead of reducing friction, organizations accidentally destroy the strengths that made one or both groups successful in the first place.

Martin Fowler and Sriram Narayan described this tension well when discussing product-oriented organizations:

> "Organizations operating in product-mode use durable, ideate-build-run teams working on a persistent business issue to continuously deliver value to customers."
>
> — Martin Fowler, *Programs in Product Mode*

The mistake many acquiring organizations make is assuming those durable operating characteristics can simply be replaced through process standardization.

---

# Operating Models Are Architectural Forces

Operating models are not simply management preferences.

They directly shape:

* Team topology
* Communication paths
* Deployment patterns
* Ownership boundaries
* Governance models
* System architecture

This is [Conway’s Law](https://martinfowler.com/bliki/ConwaysLaw.html) at organizational scale.

If one company operates with:

* stream-aligned product teams
* CI/CD ownership
* domain-centric architecture
* durable team ownership

while the other operates with:

* activity-oriented teams
* centralized release management
* heavy governance
* large approval chains

then the resulting systems will naturally reflect those differences.

Trying to force both into a single model immediately usually creates organizational instability.

As Fowler and Narayan describe:

> "It is common for organizations operating in this way to have an organizational structure that mirrors their architecture."
>
> — Martin Fowler, *Programs in Product Mode*

That relationship between organizational communication and system design becomes critically important during mergers.

---

# Tooling Is Rarely the Real Problem

One of the clearest lessons I learned is that tooling debates are usually proxy wars for operating model conflicts.

The arguments appear to be about:

* work item management platforms (Jira vs ADO, etc.)
* documentation platforms (Confluence, SharePoint, etc.)
* communication mediums (email, chat, etc.)
* GitHub vs centralized SCM
* release pipelines
* approval workflows

But underneath those discussions are deeper assumptions:

* Who owns delivery?
* Who approves production changes?
* How autonomous are teams?
* Is governance proactive or reactive?
* Are teams aligned to activities or business capabilities?
* Is the organization optimizing for flow or control?

The tools simply expose those differences.

In many acquisitions, the tooling debate becomes a surrogate for a much larger argument about organizational trust.

---

# Activity-Oriented vs Business-Capability-Centric

The largest divide I encountered was between two fundamentally different organizational philosophies.

## Activity-Oriented Organizations

These organizations optimize around:

* specialized functions
* centralized governance
* handoffs
* standardized processes
* resource pooling
* offshore scaling
* operational control

Examples include:

* centralized testing teams
* separate deployment teams
* ticket-driven infrastructure
* architecture review gates
* release management offices

This model can work reasonably well for:

* large compliance-heavy environments
* predictable delivery patterns
* highly centralized organizations

But it tends to create:

* slower flow
* larger coordination overhead
* weaker ownership
* tightly coupled systems

Martin Fowler’s article on activity-oriented organizations describes the tradeoff directly:

> "Activity-oriented teams are prone to optimize for their own activity and not for the bigger picture of delivering useful software."
>
> — Martin Fowler, *Activity-Oriented Organizations*

Another important observation:

> "Organizing by activity gets in the way of lowering batch size of work that is handed-off between teams."
>
> — Martin Fowler, *Activity-Oriented Organizations*

That is exactly the behavior many organizations unintentionally amplify after acquisitions.

## Business-Capability-Centric Organizations

These organizations optimize around:

* durable ownership
* business outcomes
* product thinking
* autonomous delivery
* end-to-end accountability
* rapid feedback loops

Teams typically own:

* infrastructure
* testing
* deployment
* observability
* operational support
* domain architecture

This model tends to produce:

* faster learning
* better architectural cohesion
* higher deployment frequency
* stronger accountability
* lower coordination overhead

But it requires significant organizational trust.

As Fowler describes in *Products Over Projects*:

> "A team gets funded."
>
> — Martin Fowler, *Products Over Projects*

That sounds deceptively simple, but it fundamentally changes ownership models, incentives, and long-term architectural evolution.

---

# Why Standardization Often Fails

In acquisitions, one operating model usually becomes dominant.

The dominant organization often unintentionally encodes its assumptions into:

* tooling
* governance
* workflow states
* reporting structures
* approval models
* architectural standards

The other organization then experiences growing friction.

Their teams appear:

* slower
* resistant
* fragmented
* misaligned

But often the real issue is structural mismatch.

The organization is measuring one operating model using metrics designed for another.

In many cases, leadership mistakes reduced autonomy for improved alignment.

But alignment created through forced process standardization is often fragile.

---

# Conway’s Law Always Wins

One of the hardest truths in enterprise architecture is this:

You cannot separate organizational structure from system architecture.

Eventually the systems mirror the communication structure of the organization.

If organizations:

* centralize decision making
* fragment ownership
* create approval-heavy delivery
* split responsibilities across many teams

their systems become:

* tightly coupled
* difficult to evolve
* coordination-heavy
* slow to deploy

Likewise, when organizations align around:

* bounded contexts
* durable ownership
* stream-aligned teams
* platform enablement

their systems evolve differently.

This is why organizational integration strategy matters more than most technical integration strategies.

A merger may consolidate systems relatively quickly.

But if the communication model remains fragmented, the architecture eventually reflects that fragmentation.

---

# The Better Strategy: Align Objectives, Not Everything Else

The most successful approach I have seen is not immediate operational unification.

Instead:

* align around principles
* align around outcomes
* align around architectural direction
* align around governance intent

while allowing operating models to remain intentionally different where appropriate.

This means accepting that:

* different SDLC models may coexist
* different team topologies may coexist
* different governance approaches may coexist
* different tooling patterns may coexist

for a significant period of time.

That is not failure.

That is realism.

As Fowler noted when discussing programs in product-oriented organizations:

> "Programs — where delivering customer value demands orchestration across multiple teams — are a real challenge for product-mode organizations."
>
> — Martin Fowler, *Programs in Product Mode*

Acquisitions magnify those coordination challenges significantly.

---

# Shared Principles Matter More Than Shared Process

The healthiest mergers I have seen focused on shared principles instead of forcing identical execution models.

Examples:

* API-first integration
* domain ownership
* automation-first delivery
* observability standards
* infrastructure as code
* bounded contexts
* platform enablement
* deployment automation
* security guardrails

Those principles create alignment without forcing every team into identical workflows.

One of the most important organizational shifts is moving away from measuring local optimization.

As Fowler observed:

> "Activity-oriented organization may be attractive from the perspective of maximizing utilization but it comes in the way of maximizing value-addition and end-to-end responsiveness."
>
> — Martin Fowler, *Activity-Oriented Organizations*

That distinction becomes critical during post-acquisition integration.

---

# Platform Teams Instead of Centralized Control

One of the more effective patterns I have seen is transforming centralized operational groups into platform teams.

Instead of:

* ticket queues
* deployment approvals
* infrastructure handoffs
* centralized release ownership

platform teams provide:

* self-service infrastructure
* CI/CD tooling
* observability
* security baselines
* reusable capabilities
* automation guardrails

This allows multiple operating models to coexist while still maintaining enterprise consistency.

Healthy platform organizations reduce friction instead of becoming centralized gatekeepers.

Their purpose is enablement.

Not control.

---

# Governance Through Visibility, Not Friction

Organizations often assume mergers require more approval layers.

In practice, excessive governance friction usually slows integration efforts dramatically.

A better approach is:

* transparent reporting
* policy automation
* architectural visibility
* observability
* deployment telemetry
* auditability

This creates trust without creating bottlenecks.

The goal should be:
high visibility with low friction.

> We found that external approvals were negatively correlated with lead time, deployment frequency, and restore time, and had no correlation with change fail rate. In short, approval by an external body (such as a manager or CAB) simply doesn’t work to increase the stability of production systems, measured by the time to restore service and change fail rate. However, it certainly slows things down. It is, in fact, worse than having no change approval process at all.
>
> — *Accelerate: The Science of Lean Software and DevOps* (Nicole Forsgren, Jez Humble, Gene Kim)

Many enterprise organizations still underestimate how much coordination friction impacts delivery performance.

---

# The Most Important Lesson

The biggest lesson I learned from operating model integration is this:

You cannot force trust, autonomy, and product ownership into existence through process frameworks.

Those are organizational and leadership decisions.

If leadership fundamentally distrusts teams, then:

* project-mode dominates
* approvals multiply
* centralized governance expands
* coordination overhead grows
* architecture quality degrades

No tooling migration or framework adoption will solve that.

As Fowler wrote in *Products Over Projects*:

> "For building, running and iterating on the solution or even pivoting to a different solution till the underlying problem is verifiably solved."
>
> — Martin Fowler, *Products Over Projects*

That level of ownership cannot exist in organizations built entirely around temporary delivery structures and fragmented accountability.

---

# Final Thoughts

Acquisitions often fail technologically not because the systems are incompatible, but because the organizations are.

The most successful long-term integrations I have seen:

* respected operating model differences
* aligned around outcomes instead of process
* invested in platform capabilities
* preserved durable ownership
* reduced unnecessary coordination
* optimized for flow instead of control

The organizations that struggled most were the ones attempting to standardize everything immediately.

Integration should focus on:

* shared direction
* shared principles
* shared trust

not forced uniformity.

Because in the end, architecture follows communication structures.

And communication structures follow organizational design.

Conway’s Law always wins.

---

# References

* [Martin Fowler — Programs in Product Mode](https://martinfowler.com/articles/programs-in-product-mode.html)
* [Martin Fowler — Activity-Oriented Organizations](https://martinfowler.com/bliki/ActivityOriented.html)
* [Martin Fowler — Business Capability Centric Organizations](https://martinfowler.com/bliki/BusinessCapabilityCentric.html)
* [Martin Fowler — Outcome-Oriented Organizations](https://martinfowler.com/bliki/OutcomeOriented.html)
* [Martin Fowler — Products Over Projects](https://martinfowler.com/articles/products-over-projects.html)
* [Martin Fowler — Team Topologies](https://martinfowler.com/bliki/TeamTopologies.html)
* [Martin Fowler — Conway's Law](https://martinfowler.com/bliki/ConwaysLaw.html)
* Eric Evans — *Domain-Driven Design*
* Matthew Skelton & Manuel Pais — *Team Topologies*
* Forsgren, Humble, Kim — *Accelerate: The Science of Lean Software and DevOps*
* Tradable Quality Hypothesis
* Design Stamina Hypothesis
