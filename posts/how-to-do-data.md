# How to Do Data

A lot of content about data falls into one of two traps. You get
tactical tool tutorials, or you get platitudes about being
"data-driven" that don't tell you how to actually execute.

This is an attempt at something in between, a framework for thinking
about what happens after the data lands in the warehouse.

---

## The real problem isn't the data

Most teams that struggle with data aren't struggling because the data
is missing. They're struggling because the meaning behind it is
implicit, living in someone's head, a Slack thread from 18 months
ago, or a spreadsheet that predates the current analytics stack.

The political fights over metric definitions, the stalemates on
dashboard ownership, the "why does your number say X when mine says
Y" conversations, these aren't data quality problems. They're semantic
problems. And they don't get solved by adding another tool.

---

## Data as a value chain

The most useful framing I've found is to think about data work in
three phases, not as job titles or tool categories, but as distinct
promises to downstream customers.

**DataOps** is farming. The promise is fresh, clean, consistently
updated ingredients. Without this, nothing else works. But it's
table stakes, not the destination.

**MetricsOps** is the kitchen. Trained people take those ingredients
and develop recipes, agreed-upon definitions of how things are
calculated, what they're called, and why. This is where most teams
underinvest. It's hard because it requires both technical judgment and
business intuition simultaneously, and it's political because metrics
are proxies for accountability.

**ProductOps** is the front of house. It's how the output reaches the
person who needs it, in the right format, at the right time, with
enough context to act on it. Self-service BI, operational analytics,
customer-facing dashboards, and ML pipelines all live here.

Each phase has a distinct customer and a distinct failure mode. Most
data teams try to run all three at once without distinguishing between
them, which is why everything feels perpetually behind.

---

## The GPS analogy

Data should work like navigation. Not just "here's where you are"
but "here's where you're going, here's the fastest route, and here's
what changed since you last checked."

That requires two things most teams skip. You need to map the roads,
meaning your actual business processes, documented and understood, and
you need to model the traffic, meaning how data flows through those
processes, where it congests, where it's missing.

Without the map, you're giving people coordinates with no street
names.

---

## Data as intuition

The goal of the MetricsOps phase, and really the goal of the data
function overall, is to develop enough intuition about the business
that the models start to match what domain experts already know to be
true. When that happens, two things occur. Stakeholders trust the
numbers, and the gaps in their own understanding become visible in a
way they couldn't see before.

That trust compounds. It's the difference between a data team that
fields requests and one that shapes decisions.

---

## Why this matters more now

This framework predates the current AI moment, but the AI moment
makes it more urgent, not less.

When AI agents start consuming your data, answering questions,
generating reports, surfacing anomalies, they inherit every implicit
assumption, undocumented join, and contested metric definition in your
stack. The agent doesn't know that "revenue" means something different
to marketing than it does to finance. It doesn't know that a column
was renamed eight months ago and the old name is still referenced in
three downstream models.

The semantic layer is not a new problem. AI just made the cost of
ignoring it impossible to defer.

DataOps, MetricsOps, ProductOps, in that order, with intention.

That's how you do data.
