---
title: "Is SAFe the Right Fit?"
date: 2026-05-08
tags: [architecture, agile, safe, conways-law, team-topologies, product-mode]
excerpt: "SAFe can improve reporting and coordination in the short term, but in many organizations it becomes a mechanism for preserving activity-based structures instead of enabling true agility."
published: true
---

Over the years, I have worked with organizations attempting to “become agile” while still preserving traditional operating models, governance structures, approval chains, and project funding practices. In many of those environments, the Scaled Agile Framework (SAFe) was introduced as the solution.

In practice, I have rarely seen SAFe solve the underlying problem.

What I *have* seen is organizations using SAFe as a way to avoid confronting deeper organizational and architectural issues:

- [Conway’s Law misalignment](/Conways-Law/)
- Project-based funding models
- Activity-oriented organizational structures
- Lack of trust in product ownership
- Centralized governance bottlenecks
- Weak domain ownership
- Large handoff-oriented delivery models

SAFe often becomes a coordination layer wrapped around those existing problems rather than a mechanism that resolves them.

As Martin Fowler describes in *Activity-Oriented Organizations*:

> “Activity-oriented organizations optimize for functional efficiency instead of customer outcomes.”

That pattern is extremely common in enterprise SAFe transformations. The framework becomes an overlay on top of siloed operating structures rather than a catalyst for redesign.

<img width="1408" height="768" alt="image" src="https://github.com/user-attachments/assets/72bd9061-66a4-4429-b69a-d33de30b7e81" />

This article builds on concepts discussed in:
- [Conway’s Law and Reverse Conway Maneuver](/Conways-Law/)
- [Merging Two Operating Models](/Merging-Two-Operating-Models/)

---

# The Appeal of SAFe

To be fair, SAFe solves real problems for leadership.

In large enterprises, executives often struggle with:
- Planning visibility
- Budget forecasting
- Cross-team coordination
- Governance consistency
- Vendor management
- Compliance reporting
- Dependency management

SAFe provides a framework that makes those concerns easier to manage organizationally.

In the first year especially, leadership usually feels relief:
- Better reporting
- Standardized ceremonies
- Centralized planning
- Predictable release trains
- Cleaner portfolio dashboards

From a management perspective, it feels like progress.

But many organizations confuse improved coordination with improved agility.

Those are not the same thing.

Martin Fowler captured this distinction well in *Programs in Product Mode*:

> “The shift from project to product is fundamentally a shift from temporary delivery structures to persistent ownership.”

SAFe implementations often improve visibility while still preserving temporary project-oriented thinking underneath.

---

# SAFe Often Optimizes for Coordination Over Flow

One of the recurring patterns I have observed is that SAFe tends to reinforce activity-oriented operating models rather than outcome-oriented ones.

Instead of reducing dependencies, organizations frequently use SAFe to manage dependencies at scale.

That distinction matters.

There is a major difference between:
- designing systems and teams to minimize coordination needs
- creating larger coordination structures to compensate for tightly coupled systems

The first approach improves flow.

The second institutionalizes complexity.

This is where Conway’s Law becomes unavoidable.

Organizations structured around:
- centralized governance
- horizontal teams
- shared services
- approval chains
- project funding
- release management offices

will naturally produce systems reflecting those same communication structures.

The result is usually:
- tightly coupled systems
- centralized databases
- release coordination overhead
- slow deployments
- architectural friction
- unclear ownership boundaries

SAFe can manage that complexity operationally, but it does not necessarily reduce it architecturally.

Martin Fowler described the alternative in *Business Capability Centric Organizations*:

> “Organizations should be aligned around business capabilities rather than technology layers or activities.”

That alignment dramatically reduces coordination overhead because ownership boundaries become clearer both organizationally and architecturally.

---

# The Hidden Cost: Cognitive Load

One of the biggest long-term issues with SAFe is cognitive load.

As organizations scale coordination layers:
- PI planning
- ART synchronization
- dependency management
- governance reviews
- architecture review boards
- approval workflows
- portfolio alignment meetings

teams spend increasing amounts of time managing the system around delivery instead of delivering value.

Strong teams become slower because they inherit the coordination burden of weaker or more fragmented organizational structures.

Matthew Skelton and Manuel Pais describe this directly in *Team Topologies*:

> “Cognitive load is a limiting factor for teams.”

The more coordination structures organizations introduce, the more cognitive capacity gets consumed by the mechanics of delivery instead of solving customer problems.

This creates an especially painful outcome in organizations that previously had highly autonomous, stream-aligned teams.

Over time:
- deployment frequency drops
- lead time increases
- ownership becomes diluted
- innovation slows
- teams become risk-averse
- architecture quality degrades

The organization becomes optimized for predictability instead of adaptability.

This is where the research from *Accelerate* becomes particularly important.

Forsgren, Humble, and Kim found that elite-performing organizations were able to achieve both higher stability and higher throughput simultaneously.

Some of the findings that directly contradict common enterprise assumptions include:

- High performers deploy code **multiple times per day**
- High performers have **lead times measured in hours instead of weeks**
- High performers recover from incidents significantly faster
- Change failure rates are *lower*, not higher, in fast-moving organizations

One of the most important conclusions from *Accelerate* was:

> “Speed and stability are not tradeoffs.”

Many enterprise governance models implicitly assume the opposite.

Large coordination-heavy frameworks often optimize for perceived safety while unintentionally reducing both adaptability and actual delivery performance.

---

# SAFe and the Illusion of Agility

Many organizations adopting SAFe still operate fundamentally in waterfall patterns.

The terminology changes:
- projects become “epics” or "initiatives"
- phases become “program increments”
- release planning becomes “PI planning”

But structurally, very little changes.

Funding remains project-oriented.

Architecture remains centralized.

Teams remain activity-oriented.

Product owners remain backlog coordinators rather than empowered business leaders.

The organization talks about agility while preserving the same command-and-control system underneath.

This is one of the most common anti-patterns I have seen in enterprise transformations.

Martin Fowler wrote in *Products Over Projects*:

> “Projects are temporary; products require long-term ownership.”

Without changing funding and ownership models, many agile transformations simply relabel project governance using agile terminology.

---

# Product Owners Without Product Authority

A recurring issue in SAFe implementations is the treatment of Product Owners.

In healthy product-mode organizations, Product Owners:
- own business outcomes
- control prioritization
- make tradeoff decisions
- balance reliability, architecture, and features
- shape long-term product direction

In many SAFe implementations, Product Owners instead become:
- backlog administrators
- Jira managers
- dependency coordinators
- sprint planners
- status reporters

They are held accountable for outcomes without having authority over investment or strategic direction.

This disconnect creates organizational friction and weakens team autonomy.

It also undermines one of the core goals of agile delivery:
fast learning through empowered teams.

Martin Fowler describes healthy product organizations this way in *Programs in Product Mode*:

> “Persistent teams aligned to business outcomes build deeper domain knowledge and better products.”

That ownership model is difficult to achieve when decision-making remains centralized above the team level.

---

# Durable Teams vs Temporary Coordination Structures

In my experience, durable, domain-aligned, stream-aligned teams outperform large-scale coordination models over the long term.

Strong product organizations optimize for:
- bounded contexts
- clear ownership
- high cohesion
- low coupling
- autonomous deployment
- business capability alignment
- fast feedback loops

This dramatically reduces the need for centralized coordination.

When organizations instead optimize for:
- resource utilization
- shared activity teams
- project staffing pools
- centralized governance
- offshore task distribution

they increase coordination complexity.

SAFe often becomes the mechanism used to manage that growing complexity.

But managing complexity is not the same thing as reducing it.

As *Team Topologies* explains:

> “The team is the means of delivery.”

Architecture, communication structure, deployment independence, and flow efficiency all emerge from how teams are designed.

---

# Reverse Conway Maneuver Matters More Than SAFe

One of the most effective organizational strategies I have seen is the Reverse Conway Maneuver:
designing team structures intentionally around the architecture and business outcomes you want.

If you want:
- loosely coupled systems
- autonomous services
- domain ownership
- rapid delivery
- high deployment frequency

then teams themselves must reflect those boundaries.

That means:
- stream-aligned teams
- product ownership
- end-to-end accountability
- embedded quality practices
- platform enablement instead of ticket-driven infrastructure

No framework can compensate for organizational structures fundamentally working against the architecture.

This idea aligns closely with Conway’s Law itself:

> “Organizations which design systems are constrained to produce designs which are copies of the communication structures of these organizations.”

The Reverse Conway Maneuver intentionally uses that reality to improve architectural outcomes instead of fighting against it.

> See [The Reverse Conway Maneuver](/Conways-Law/) for additional details.

---

# Governance Without Bottlenecks

One of the biggest misconceptions in large enterprises is that governance requires approvals and centralized control.

The highest-performing organizations I have worked with instead rely on:
- automation
- observability
- policy guardrails
- peer review
- deployment pipelines
- progressive delivery
- rapid rollback capability

Governance becomes transparent and measurable rather than approval-driven.

This aligns closely with findings from *Accelerate*, which showed that external approval processes negatively correlate with software delivery performance.

Forsgren, Humble, and Kim found that:

> “Approval processes are positively correlated with burnout and negatively correlated with performance.”

That finding challenges a deeply embedded assumption in many enterprise governance models.

Organizations become safer not by slowing down changes, but by:
- improving detection
- improving recovery
- reducing batch sizes
- increasing deployment confidence

Another important finding from *Accelerate* was that smaller batch sizes and frequent deployments reduce risk because problems become easier to isolate and recover from.

Large governance-heavy release models often create the exact opposite condition:
large risky deployments coordinated across many teams simultaneously.

---

# When SAFe Can Work

I do think SAFe can serve a purpose in certain environments.

Particularly:
- highly regulated industries
- organizations with massive dependency networks
- companies early in modernization journeys
- enterprises lacking any delivery discipline
- transitional states between legacy and product-mode

As a temporary scaffold, SAFe can create organizational consistency.

But it becomes dangerous when:
- it becomes permanent
- it replaces organizational redesign
- it reinforces project-mode thinking
- it preserves activity-based silos
- it discourages autonomy

At that point, the framework itself becomes part of the inertia.

---

# My Experience and Conclusion

The organizations I have seen move fastest long term were not the ones with the most process.

They were the ones that:
- trusted teams
- aligned ownership to business capabilities
- funded products instead of projects
- reduced handoffs
- invested in architecture
- optimized for flow over reporting
- empowered product owners
- embraced platform engineering
- minimized coordination overhead

Their systems reflected those structures.

That is Conway’s Law in action.

Martin Fowler summarized this well in *Outcome-Oriented Organizations*:

> “Outcome-oriented organizations focus on results rather than activities.”

SAFe can improve planning optics and organizational coordination. But if the underlying operating model remains project-centric and activity-oriented, the organization will continue producing tightly coupled systems and slow delivery patterns regardless of the agile terminology being used.

The data from *Accelerate* reinforces this reality:
the highest-performing technology organizations consistently optimize for:
- fast feedback
- low-friction delivery
- deployment automation
- empowered teams
- reduced handoffs
- smaller batch sizes
- continuous learning

Not heavier coordination structures.

In the end, sustainable agility comes less from frameworks and more from:
- trust
- ownership
- architecture
- organizational alignment
- empowered teams
- outcome-oriented thinking

Frameworks can support those things.

They cannot replace them.

---

# References

- [Martin Fowler — Programs in Product Mode](https://martinfowler.com/articles/programs-in-product-mode.html)
- [Martin Fowler — Activity-Oriented Organizations](https://martinfowler.com/bliki/ActivityOriented.html)
- [Martin Fowler — Business Capability Centric Organizations](https://martinfowler.com/bliki/BusinessCapabilityCentric.html)
- [Martin Fowler — Outcome-Oriented Organizations](https://martinfowler.com/bliki/OutcomeOriented.html)
- [Martin Fowler — Products Over Projects](https://martinfowler.com/articles/products-over-projects.html)
- [Martin Fowler — Team Topologies](https://martinfowler.com/bliki/TeamTopologies.html)
- Forsgren, Humble, Kim — *Accelerate: The Science of Lean Software and DevOps*
- Eric Evans — *Domain-Driven Design*
- Matthew Skelton & Manuel Pais — *Team Topologies*
- Tradable Quality Hypothesis
- Design Stamina Hypothesis
