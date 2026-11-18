# Software Engineering Study Strategy

**11 sections · 3 study layers · about 14 hours a week**

How to run the [Software Engineering Curriculum](README.md): efficient learning, durable retention, deep mastery and strong hiring potential.

*Last updated: November 2026*

---

## How to use this guide

- **The roadmap decides what; this guide decides how.** The roadmap sets the courses, the books and their order. This guide sets how you spend each session, day and week.
- **Section numbers (§) and book numbers (#)** refer to the roadmap.
- **Read it once, then use it as a checklist.** §3–§5 are the habits you repeat every week; §8–§10 are the plans you look at when a phase starts.

---

## Contents

| # | Section | What it covers |
|---|---------|----------------|
| 1 | Core principles | What the goal is, and the mistake that wastes the most time |
| 2 | The three-layer system | How the course lane, the book lane and light reading share your time |
| 3 | Working a course | Lectures, labs, exams and placement |
| 4 | Working a book | Reading so that it sticks |
| 5 | Building | Labs, book code, milestones and side builds |
| 6 | Retention | What makes knowledge last |
| 7 | When you're stuck | The struggle rule, and using AI without losing the learning |
| 8 | Schedule | Daily templates, the weekly rhythm, reviews and rest |
| 9 | Phase by phase | Each phase's primary, secondary, light and build |
| 10 | Getting hired | The job-first variant and interview prep |
| 11 | Measuring progress | Outputs to track and each phase's exit criteria |

---

## 1 · Core principles

The goal is not the most hours, the most books or the most tutorials. The goal is deep understanding, long-term retention, practical engineering ability, employability and sustainable growth.

**The biggest mistake** is studying everything a little, every day:

❌ 1h Java · 1h DSA · 1h OS · 1h networking · 1h math

You feel busy, but every switch costs warm-up time, nothing goes deep enough to stick, and progress crawls. The fix is the three-layer system: few subjects at a time, each with a clear role.

---

## 2 · The three-layer system

The roadmap's two lanes are the first two layers.

| Layer | Share | Hours (of 14) | In the roadmap | What it looks like |
|-------|-------|---------------|----------------|--------------------|
| **Primary: deep focus** | ~60% | 8–9 | The course lane: one course at a time | Lectures, then labs, problem sets and exams. Hard, focused, no multitasking |
| **Secondary: craft** | ~30% | 4–5 | The book lane: one book at a time from the same phase | Read, then type, run and change the examples. Feed what you learn into your milestone repo |
| **Light: exposure** | ~10% | 1–2 | Reference books, talks, engineering blogs, papers | Low pressure. Builds intuition and vocabulary. No memorizing |

Rules:
- One primary and one secondary at a time. Finish one, or drop it on purpose, before starting the next.
- The primary lane's labs are your main building time. Don't skip them to read ahead.
- Light material must never turn into a second primary.

---

## 3 · Working a course

| Step | What to do |
|------|------------|
| Before each lecture | Skim its notes or slides for five minutes so you know where it's going |
| During | Watch at a speed where you can still predict the next step (often 1.25–1.5×). Pause before each worked example and try it yourself |
| After | Close everything and write the key ideas from memory, then check what you missed |
| Labs | Start them the day you reach them. Read the whole handout first, commit often, run the tests. The labs are the course |
| Exams | Sit the midterm at the halfway point and the final at the end, timed. Grade yourself with the posted solutions, then redo every missed problem a week later |
| Placement | Think you already know a topic? Sit the course's final cold. Score 80% or more and you can skip the course. Otherwise take it, but move fast through the units you aced |

---

## 4 · Working a book

| Step | What to do |
|------|------------|
| Survey (15 minutes) | Read the contents, the preface and the chapter summaries first, so you know the book's map |
| Each chapter | One chapter per session. Type and run every example in a book repo, then change one thing and predict the result before you run it |
| After each chapter | A three-sentence summary from memory, and at most three flashcards |
| After the book | A one-page summary, plus one concrete change in your milestone repo because of what you read |
| Reference books | Read only the chapters for your current problem. Note where you stopped and come back later |
| Older-version books | Run the examples on the current Java or Spring release and fix what breaks. The fixes teach you what changed |

---

## 5 · Building

Without implementation, concepts stay abstract and fade within weeks. The roadmap builds at three levels:

1. **Labs and problem sets, every week.** Gitlet, the 15-213 labs, xv6, BusTub, Raft. They come with tests, so you know when you're right.
2. **Book code, every book.** A book you only read is a book you'll forget.
3. **Milestones, every phase.** The JVM HTTP server, the production-grade Spring Boot service, the distributed split, then running it in production. Phases 3–5 grow one system, which becomes your portfolio.

**A milestone is done when:**
- it works end to end, from a clean checkout, with one command;
- its tests run in CI and pass;
- its README explains the design decisions and the trade-offs you rejected;
- you've measured one thing that matters (latency, throughput or recovery time) and written down the number.

**Side builds** give you more reps between milestones. Start one once its phase has given you the tools: a URL shortener or WebSocket chat in Phase 3, an OAuth2 auth service after §11, a caching layer or distributed rate limiter in Phase 4.

---

## 6 · Retention

Retention comes from retrieving and using knowledge, not from re-reading it.

| Technique | How |
|-----------|-----|
| Active recall | After every lecture or chapter, write the key ideas from memory before you look back |
| Spaced repetition | A small Anki deck for things worth memorizing: complexities, isolation anomalies, syscalls, HTTP semantics, Java memory-model rules. Write cards in your own words; ten minutes a day |
| Explain it | Write a short note as if teaching it. The parts you can't explain are the parts you don't understand yet |
| Re-implement | A week after a lab, rebuild its core from a blank file without looking |
| Timed exams | Covered in §3. Redoing the misses is where most of the value is |
| Debug your own code | The bugs you chase down yourself are the lessons you keep |

What doesn't work: passive re-reading, highlighting, binge-watching lectures without doing the labs, hopping between tutorials.

**Notes.** Keep one short note per concept, in your own words, linked to its source. Keep a **mistake log** too: every bug that cost you more than an hour, with its cause and fix. Reread it before exams and interviews; it doubles as your bank of interview stories.

---

## 7 · When you're stuck

1. **Struggle first, for 30–45 minutes.** Productive struggle is where the learning happens.
2. Reread the relevant notes or chapter. Shrink the problem; write a failing test.
3. Then take hints: the course's hints, docs, search, or an AI tutor.
4. If you read a full solution, close it and re-solve from scratch the next day.

**Using AI without losing the learning:**
- **Do** ask it to explain a concept another way, quiz you, review code you already wrote, or give a hint after you've genuinely tried.
- **Don't** let it write lab code or solve problem sets before you have. Passing labs with generated code teaches you nothing, and the exams will show it.

---

## 8 · Schedule

### Daily templates

| Day length | Deep (course lane) | Practical (labs, milestone) | Book lane | Review |
|------------|--------------------|-----------------------------|-----------|--------|
| 2 hours | 75m | — | 30m | 15m |
| 3 hours | 90m | 50m | 25m | 15m |
| 4 hours | 2h | 75m | 30m | 15m |
| 5 hours | 2h | 90m | 75m | 15m |
| 6 hours | 2.5h | 90m | 90m | 30m |

Deep sessions run 90–120 minutes on one hard thing, with your phone away. Stop at a natural checkpoint and write one line on where to resume. Past about six focused hours, returns drop sharply: rest instead.

### Weekly rhythm

| Day type | Hours | Content |
|----------|-------|---------|
| Heavy | 4–6h | Long lab or milestone sessions |
| Medium | 2–3h | Lectures, the book lane, a few EPI problems |
| Light | 1–2h | Reading and the weekly review |
| Rest | 0 | Nothing. Really |

A typical 14-hour week: one heavy day (5h), three medium days (2.5h each), one light day (1.5h), two rest days.

### Reviews and rest

| Cadence | Time | What |
|---------|------|------|
| Daily | 10–15m | End every study day with recall and flashcards |
| Weekly | 30m | What did I learn? What's still unclear? What is next week's one primary goal? |
| Monthly | 30m | Retro: what stuck, what didn't, what to change. Adjust the plan, not your standards |
| Every 6–8 weeks | 1 week | Deload: only review, light reading and redoing missed problems. It prevents burnout and consolidates memory |

---

## 9 · Phase by phase

| Phase | Primary (course lane) | Secondary (book lane) | Light | Build |
|-------|-----------------------|-----------------------|-------|-------|
| 0 · Toolkit | Missing Semester | — | — | Your dev setup and dotfiles in Git |
| 1 · Foundations | CS61B → 6.042J → 6.006 | Core Java I → Effective Java → Kotlin (#1–#4) | EPI problems weekly (#9) | Gitlet, then a Kotlin port |
| 2 · Systems and Craft | 15-213 → 6.1810 → CS168 | Concurrency → design → testing (§6–§8) | Systems Performance (#18), talks | The labs, then the JVM HTTP server |
| 3 · Backend Engineering | Spring Academy → 15-445 → CS161 | Spring → persistence → security (§9–§11) | PoEAA (#38), OWASP cheat sheets | Production-grade Spring Boot service |
| 4 · Distributed Systems and Architecture | Cambridge DS → 6.5840 → Confluent | DS → architecture → DDD → microservices → events (§12–§16) | Papers, engineering blogs | 6.5840 labs, then split the service |
| 5 · Production and Staff-Level Practice | DevOps with Docker → DevOps with Kubernetes → 6.033 | §17 → §18 → §19 | Postmortems, SRE blogs | Run it in production |

**Where math fits.** Math gets one focused stint, not a permanent slot. 6.042J is your primary for its 3–4 months because 6.006 depends on it: proofs, induction, asymptotics, counting and basic probability. After that, math stays in the light layer. Reach for Dekking (#7) or Stat 110 when you need statistics for benchmarks, latency percentiles or experiments.

---

## 10 · Getting hired

### Highest-ROI topics (2026)

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

### Job-first variant

The roadmap starts from first principles, so Spring doesn't arrive until Phase 3. If you need a backend job sooner, reorder instead of skipping:

1. **Phase 0, then CS61B** with Core Java I (#1) and Effective Java (#2). About 4 months.
2. **Fast track, about 3–4 months.** Spring Academy, Spring in Action (#28), The Art of PostgreSQL (#35), the core chapters of High-Performance Java Persistence (#36), and DevOps with Docker. Build a smaller version of the Phase 3 service: REST, PostgreSQL, tests, Docker. Work EPI problems (#9) daily.
3. **Start applying.** The fast-track service is your portfolio piece.
4. **Resume the roadmap at 6.042J** and continue in order, skipping what the fast track already covered.

The deep material still happens; it just comes after you're earning.

### Before any interview loop (6–8 weeks)

- EPI problems (#9) daily, timed, out loud.
- System Design Interview Vol. 1–2 (#65–#66), then practise designs against a clock.
- Mock interviews, at least one a week.
- Rehearsed stories from your milestones and mistake log: what you built, what broke, what you'd change.

---

## 11 · Measuring progress

Track outputs, not hours.

| Unit | Done when |
|------|-----------|
| Course | Its labs pass their tests, and your timed final, graded with the posted solutions, is 70% or better |
| Book | You've written the one-page summary and made the change it inspired in your repo |
| Milestone | It meets the definition of done in §5 |
| Phase | Its core courses, its book lane and its milestone are all done. Only then start the next phase |

---

## Summary

1. One primary subject (the course lane) and one secondary (the book lane).
2. Build constantly: labs every week, code with every book, a milestone every phase.
3. Retrieve, don't re-read: recall, spaced repetition, re-implementation, timed exams.
4. Keep context switching to a minimum.
5. Math gets one deep stint, then stays light.
6. Consistency over intensity: rest days and deload weeks are part of the plan.
7. Need a job soon? Take the job-first variant, then return to the roadmap.

---

*Memento Mori. Memento Vivere.*

