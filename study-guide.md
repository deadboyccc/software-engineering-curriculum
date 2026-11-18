# Software Engineering Study Strategy

> How to run the Software Engineering Curriculum: efficient learning, durable retention, deep mastery, strong hiring potential.

The roadmap decides **what** to learn and in what order. This guide decides **how** you spend each day and week.

---

## Core philosophy

The goal is not:
- studying the most hours
- reading the most books
- consuming endless tutorials

The goal is:
- deep understanding
- long-term retention
- practical engineering ability
- employability
- sustainable growth

---

## The biggest mistake

Studying everything a little, every day.

❌ 1h Java · 1h DSA · 1h OS · 1h networking · 1h math

You feel busy, but every switch costs warm-up time, nothing goes deep enough to stick, and progress crawls.

The fix: few subjects at a time, each with a clear role.

---

## The three-layer system

The roadmap's two lanes are the first two layers.

| Layer | Share | In the roadmap | What it looks like |
|-------|-------|----------------|--------------------|
| **Primary: deep focus** | ~60% | The course lane: one course at a time | Lectures, then labs, problem sets and exams. Hard, focused, no multitasking |
| **Secondary: craft** | ~30% | The book lane: one book at a time from the same phase | Read, then type, run and change the examples. Feed what you learn into your milestone repo |
| **Light: exposure** | ~10% | Reference books, talks, engineering blogs, papers | Low pressure. Builds intuition and vocabulary. No memorizing |

Rules:
- One primary and one secondary at a time. Finish one, or drop it on purpose, before starting the next.
- The primary lane's labs are your main building time. Don't skip them to read ahead.
- Light material must never turn into a second primary.

---

## The most important rule: build while learning

Without implementation, concepts stay abstract and fade within weeks. In the roadmap, building happens at three levels:

1. **Labs and problem sets, every week.** Gitlet, the 15-213 labs, xv6, BusTub, Raft. They come with tests, so you know when you're right.
2. **Book-lane code, every book.** Type, run and break the examples. A book you only read is a book you'll forget.
3. **Milestones, every phase.** The JVM HTTP server, the production-grade Spring Boot service, the distributed split, then running it in production. Phases 3–5 grow one system, which becomes your portfolio.

Want more reps between milestones? Build a side project once its phase has given you the tools: a URL shortener or WebSocket chat in Phase 3, an OAuth2 auth service after §11, a caching layer or distributed rate limiter in Phase 4.

Projects give you retention, intuition, portfolio proof and interview stories.

---

## Highest-ROI topics for backend hiring (2026)

| Topic | Where it lives in the roadmap |
|-------|-------------------------------|
| Java | §1, §6 |
| Spring Boot | §9 |
| Real backend projects | Milestones, Phases 3–5 |
| PostgreSQL and SQL | §10 |
| Data structures and algorithms | §1, §3, #9 |
| Testing | §8 |
| Docker and Kubernetes | §17 |
| Linux | Phase 0, §4 |
| OS and networking fundamentals | §4, §5 |
| Kafka and distributed systems | §12, §16 |

If hiring speed is your top priority, use the [job-first variant](#job-first-variant).

---

## Where math fits

Math gets one focused stint, not a permanent slot.

- **6.042J is your primary for its 3–4 months**, because 6.006 depends on it: proofs, induction, asymptotics, counting, basic probability. Do it properly, then move on.
- **After that, math stays in the light layer.** Reach for Dekking (#7) or Stat 110 when you need statistics for benchmarks, latency percentiles or experiments.
- You don't need heavy statistics or advanced proof techniques for backend work.
- The roadmap's math book is *Mathematics for Computer Science* (#6), the 6.042J text. It replaced Epp.

---

## Session types

### Deep session: 90–120 minutes
One hard thing from the primary lane: a lecture with its notes, or a lab. Phone away, one window. Stop at a natural checkpoint and write one line on where to resume.

### Practical session: 60–90 minutes
Implementation only: labs, book-lane code, milestone work, debugging. This is where retention happens.

### Light session: 20–40 minutes
Book-lane reading, a reference chapter, a talk or a paper. Good for tired evenings.

### Review: 10–20 minutes
Close the material and recall it (see [retention](#how-retention-actually-works)). End every study day with one.

---

## Daily templates

The roadmap assumes about 14 hours a week. Pick the template that fits the day.

**2 hours**

| Block | Time |
|-------|------|
| Primary (lecture or lab) | 75m |
| Secondary (book) | 30m |
| Review | 15m |

**3 hours**

| Block | Time |
|-------|------|
| Primary deep session | 90m |
| Practical (lab or book code) | 50m |
| Secondary (book) | 25m |
| Review | 15m |

**4 hours**

| Block | Time |
|-------|------|
| Primary deep session | 2h |
| Practical (lab or milestone) | 75m |
| Secondary (book) | 30m |
| Review | 15m |

**5 hours**

| Block | Time |
|-------|------|
| Primary deep session | 2h |
| Practical (lab or milestone) | 90m |
| Secondary (book) | 75m |
| Review | 15m |

**6 hours**

| Block | Time |
|-------|------|
| Primary deep session | 2.5h |
| Practical (lab or milestone) | 1.5h |
| Secondary (book) | 1.5h |
| Review | 30m |

Past about six focused hours, returns drop sharply. Spend extra time resting, not studying.

---

## Weekly rhythm

| Day type | Hours | Content |
|----------|-------|---------|
| Heavy | 4–6h | Long lab or milestone sessions |
| Medium | 2–3h | Lectures, the book lane, a few EPI problems |
| Light | 1–2h | Reading and the weekly review |
| Rest | 0 | Nothing. Really |

A typical 14-hour week: one heavy day (5h), three medium days (2.5h each), one light day (1.5h), two rest days.

- **Weekly review (30 minutes, on the light day).** What did I learn? What's still unclear? What is next week's one primary goal?
- **Deload week every 6–8 weeks.** Only review, light reading and redoing missed problems. It prevents burnout and consolidates memory.

---

## How retention actually works

Retention comes from retrieving and using knowledge, not from re-reading it.

What works:
1. **Active recall.** After each lecture or chapter, close it and write the key ideas from memory. Then check what you missed.
2. **Spaced repetition.** Keep a small Anki deck for things worth memorizing: complexities, isolation anomalies, syscalls, HTTP semantics, Java memory-model rules. Write cards in your own words; ten minutes a day.
3. **Explain it.** Write a short note as if teaching it. The parts you can't explain are the parts you don't understand yet.
4. **Re-implement from a blank file.** A week after a lab, rebuild its core without looking.
5. **Exams as checkpoints.** Sit each course's midterm and final timed, grade yourself with the solutions, then redo every missed problem a week later.
6. **Debug your own code.** The bugs you chase down yourself are the lessons you keep.

What doesn't work: passive re-reading, highlighting, binge-watching lectures without doing the labs, hopping between tutorials.

### Notes
- One short note per concept, in your own words, linked to its source.
- A **mistake log**: every bug that cost you more than an hour, with its cause and fix. Reread it before exams and interviews; it doubles as your bank of interview stories.

---

## When you're stuck

1. **Struggle first, for 30–45 minutes.** Productive struggle is where the learning happens.
2. Reread the relevant notes or chapter. Shrink the problem; write a failing test.
3. Then take hints: the course's hints, docs, search, or an AI tutor.
4. If you read a full solution, close it and re-solve from scratch the next day.

### Using AI without losing the learning
- **Do** ask it to explain a concept another way, quiz you, review code you already wrote, or give a hint after you've genuinely tried.
- **Don't** let it write lab code or solve problem sets before you have. Passing labs with generated code teaches you nothing, and the exams will show it.

---

## The rotation, phase by phase

This follows the roadmap's phases.

| Phase | Primary (course lane) | Secondary (book lane) | Light | Build |
|-------|-----------------------|-----------------------|-------|-------|
| 0 · Toolkit | Missing Semester | — | — | Your dev setup and dotfiles in Git |
| 1 · Foundations | CS61B → 6.042J → 6.006 | Core Java I → Effective Java → Kotlin (#1–#4) | EPI problems weekly (#9) | Gitlet, then a Kotlin port |
| 2 · Systems and Craft | 15-213 → 6.1810 → CS168 | Concurrency → design → testing (§6–§8) | Systems Performance (#18), talks | The labs, then the JVM HTTP server |
| 3 · Backend Engineering | Spring Academy → 15-445 → CS161 | Spring → persistence → security (§9–§11) | PoEAA (#38), OWASP cheat sheets | Production-grade Spring Boot service |
| 4 · Distributed Systems | Cambridge DS → 6.5840 → Confluent | DS → architecture → DDD → microservices → events (§12–§16) | Papers, engineering blogs | 6.5840 labs, then split the service |
| 5 · Production | DevOps with Docker → DevOps with Kubernetes → 6.033 | §17 → §18 → §19 | Postmortems, SRE blogs | Run it in production |

---

## Job-first variant

The roadmap starts from first principles, so Spring doesn't arrive until Phase 3. If you need a backend job sooner, reorder instead of skipping:

1. **Phase 0, then CS61B** with Core Java I (#1) and Effective Java (#2). About 4 months.
2. **Fast track, about 3–4 months.** Spring Academy, Spring in Action (#28), The Art of PostgreSQL (#35), the core chapters of High-Performance Java Persistence (#36), and DevOps with Docker. Build a smaller version of the Phase 3 service: REST, PostgreSQL, tests, Docker. Work EPI problems (#9) daily.
3. **Start applying.** The fast-track service is your portfolio piece.
4. **Resume the roadmap at 6.042J** and continue in order, skipping what the fast track already covered.

The deep material still happens; it just comes after you're earning.

**Before any interview loop (6–8 weeks):** EPI daily, System Design Interview Vol. 1–2 (#65–#66), mock interviews, and rehearsed stories from your milestones and mistake log.

---

## Measuring progress

Track outputs, not hours.

- **Courses:** labs pass their tests; exam scores are graded against the solutions.
- **Books:** a one-page summary, plus something you built or changed because of the book.
- **Phases:** the milestone works, has tests, and has a README explaining its design choices.
- **Monthly retro (30 minutes):** what stuck, what didn't, what to change. Adjust the plan, not your standards.

---

## Final summary

1. One primary subject (the course lane) and one secondary (the book lane).
2. Build constantly: labs every week, code with every book, a milestone every phase.
3. Retrieve, don't re-read: recall, spaced repetition, re-implementation, timed exams.
4. Keep context switching to a minimum.
5. Math gets one deep stint, then stays light.
6. Consistency over intensity: rest days and deload weeks are part of the plan.
7. Need a job soon? Take the job-first variant, then return to the roadmap.
