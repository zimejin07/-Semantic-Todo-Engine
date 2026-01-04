# Vector Todo AI

This repository is the starting point for building a **semantic todo system** that treats tasks as meaning, not strings.

The goal is to build a working system where todos are embedded as vectors and retrieved by similarity, enabling search, grouping, and reasoning based on intent rather than exact wording.

This is a build-first project. The emphasis is on producing something functional, understanding trade-offs, and iterating based on real behavior—not speculation.

---

## Why This Project

Traditional todo apps are optimized for:
- Exact text matching
- Manual categorization
- Rigid structures

This project explores a different premise:

> If todos are represented as vectors, you can search and organize them by semantic similarity.

That unlocks:
- Finding related tasks even when phrasing differs
- Grouping todos by theme or intent
- Detecting overlap and duplication
- Querying with vague or incomplete ideas and still getting useful results

---

## Core Goal

Build a todo system where:
- Todos are written in natural language
- Each todo is embedded into a vector
- Queries are also vectors
- Retrieval is based on similarity, not keywords

---

## Planned Capabilities

- [ ] Create todos as free-form text
- [ ] Convert todos into vector embeddings
- [ ] Store embeddings in a vector database
- [ ] Perform similarity search over todos
- [ ] Rank results by relevance
- [ ] Query using:
  - Natural language
  - Another todo
  - Partial or high-level intent

---

## Design Constraints

- Minimal surface area
- Clear data flow: text → embedding → vector → retrieval
- Pluggable components
- Bias toward understanding over polish

---

## Open Design Space

These questions are intentionally left open and will be answered through implementation:

- How small can a todo be before embeddings lose signal?
- Should completed todos remain searchable?
- How should metadata (priority, date, tags) interact with vectors?
- When does vector search outperform hybrid approaches?

---

## Expansion Ideas (After Core Works)

- [ ] Automatic clustering of todos
- [ ] Duplicate and near-duplicate detection
- [ ] Suggested todos based on existing ones
- [ ] Time-aware relevance decay
- [ ] Hybrid vector + keyword retrieval

---

## Scope and Expectations

- Not a production app
- Not optimized for scale
- Explicitly experimental

Progress is measured by:
- Working code
- Clear mental models
- Fewer black boxes

---

## Current Status

- Initialization phase
- Architecture intentionally flexible
- No stable API yet

---

## License

MIT.
