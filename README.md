# Software Engineering Curriculum

**69 books · 19 sections · 5 phases, plus a two-week toolkit**

A structured path from first principles to staff-level engineering, centered on the Java, Kotlin and Spring ecosystem, with deep coverage of distributed systems and engineering practice.

*Last updated: November 2026*

---

## How to use this roadmap

- **Run two lanes at once.** The *course lane* is one university course at a time, in the order given (about 8–10 hours a week). The *book lane* is one book at a time from the same phase (about 4–5 hours a week). Each phase pairs them on purpose: you read *Java Concurrency in Practice* while 6.1810 is teaching locks and scheduling, and *High-Performance Java Persistence* while 15-445 is teaching query execution.
- **Course roles.** *Core* courses are the path. *Deepen* courses are optional second passes; take one when a topic grabs you or your work needs it. *On-ramp* fills a prerequisite gap, if you have one.
- **The labs and exams are the course.** Lectures alone don't stick. Do every lab. Sit each exam timed, then grade yourself against the posted solutions.
- **Placement by exam.** If you already know a topic, take that course's final exam cold. If you pass, skip the course and keep its book as a reference.
- **Reference books** (marked in Notes) are for lookup: read the chapters you need now and come back later.
- **Older books, current platform.** Where a book targets an older Java or Spring release, take the ideas from the book and the current APIs from [dev.java](https://dev.java/learn/) and [docs.spring.io](https://docs.spring.io/).
- **Interview books** (#9, #65, #66) aren't read cover to cover. Work a few #9 problems a week, and save #65–#66 for the months before you interview.
- **Milestones.** Each phase ends with a project. Phases 3–5 grow the same system, so keep it in one repository.

*The Materials column lists what is public for self-study: lecture video, notes or readings, labs / problem sets / projects, and exams (with solutions where noted).*

---

## Contents

| Phase | Sections | Course lane | Rough duration* |
|-------|----------|-------------|-----------------|
| 0. Toolkit | — | Missing Semester | 2 weeks |
| 1. Foundations | 1–3 | CS61B → 6.042J → 6.006 | 9–11 months |
| 2. Systems and Craft | 4–8 | 15-213 → 6.1810 → CS168 | 11–13 months |
| 3. Backend Engineering | 9–11 | Spring Academy → 15-445 → CS161 | 8–10 months |
| 4. Distributed Systems and Architecture | 12–16 | Cambridge Distributed Systems → 6.5840 → Confluent | 8–10 months |
| 5. Production and Staff-Level Practice | 17–19 | DevOps with Docker → DevOps with Kubernetes → 6.033 | 6–8 months |

\*At about 14 hours a week across both lanes: roughly four years end to end. Placement by exam shortens it.

**Prerequisites are built into the order.** 6.042J comes before 6.006 (proofs, asymptotics, probability). 15-213 comes before 6.1810 (C, x86, virtual memory). 6.1810 satisfies MIT 6.5840's prerequisite (6.1800 or 6.1810). If C is new to you, do the CS50x on-ramp before 15-213. For the Go labs in 6.5840, [A Tour of Go](https://go.dev/tour/) takes a few evenings.

---

## Phase 0 · Toolkit

**Course lane:** Missing Semester. Two weeks, before anything else.

| Course | Role | Materials |
|--------|------|-----------|
| [MIT · The Missing Semester of Your CS Education](https://missing.csail.mit.edu/) | Core | Video · Notes · Exercises. Shell, Git, editors, debugging, profiling |

---

## Phase 1 · Foundations

**Course lane:** CS61B → 6.042J → 6.006.
**Book lane:** Core Java Vol. I (alongside CS61B) → Effective Java → the Kotlin for Java Developers course with Kotlin in Action → Effective Kotlin. Books #6–#8 are the companion texts for 6.042J and 6.006; start #9 once 6.006 is under way.
**Milestone:** *Gitlet*, the CS61B project: a working Git clone in Java, with commits, branches and merges. Then port its core to idiomatic Kotlin and compare the two codebases.

### 1 · Java, Kotlin and Data Structures

| Course | Role | Materials |
|--------|------|-----------|
| [UC Berkeley CS61B · Data Structures (Spring 2021)](https://sp21.datastructur.es/) | Core | Video · Notes · Labs and projects · Exams + solutions. Java |
| [JetBrains · Kotlin for Java Developers](https://www.coursera.org/learn/kotlin-for-java-developers) | Core | Video · Exercises. Follow it with the [Kotlin Koans](https://play.kotlinlang.org/koans/overview) |

| # | Title | Author(s) | Notes |
|---|-------|-----------|-------|
| 1 | [Core Java, Vol. I — Fundamentals](https://horstmann.com/corejava/) | Cay S. Horstmann | Latest edition. Read alongside CS61B |
| 2 | [Effective Java](https://openlibrary.org/isbn/9780134685991) | Joshua Bloch | 3rd ed. Covers Java up to 9; the principles still hold |
| 3 | [Kotlin in Action](https://www.manning.com/books/kotlin-in-action-second-edition) | Aigner, Elizarov, Isakova & Jemerov | 2nd ed. |
| 4 | [Effective Kotlin](https://kt.academy/book/effectivekotlin) | Marcin Moskała | |
| 5 | [Core Java, Vol. II — Advanced Features](https://horstmann.com/corejava/) | Cay S. Horstmann | Reference |

---

### 2 · Mathematics, Logic and Probability

| Course | Role | Materials |
|--------|------|-----------|
| [MIT 6.042J · Mathematics for Computer Science (Spring 2015)](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-spring-2015/) | Core | Video · Notes (#6) · Problem sets + solutions · Exams + solutions |
| [Harvard Stat 110 · Probability](http://stat110.net/) | Deepen | Video · Free textbook · Practice problems + solutions · Exams + solutions |

| # | Title | Author(s) | Notes |
|---|-------|-----------|-------|
| 6 | [Mathematics for Computer Science](https://courses.csail.mit.edu/6.042/spring17/mcs.pdf) | Lehman, Leighton & Meyer | Free. The 6.042J text |
| 7 | [A Modern Introduction to Probability and Statistics](https://link.springer.com/book/10.1007/1-84628-168-7) | F.M. Dekking et al. | The statistics half pays off in benchmarking and experiments |

---

### 3 · Algorithms

| Course | Role | Materials |
|--------|------|-----------|
| [MIT 6.006 · Introduction to Algorithms (Spring 2020)](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2020/) | Core | Video · Notes · Problem sets + solutions · Quizzes + solutions. Python |
| Princeton Algorithms: [Part I](https://www.coursera.org/learn/algorithms-part1) · [Part II](https://www.coursera.org/learn/algorithms-part2) | Deepen | Video · [Booksite](https://algs4.cs.princeton.edu/) · Autograded Java assignments. Part II's strings, max-flow and compression go past CS61B |

| # | Title | Author(s) | Notes |
|---|-------|-----------|-------|
| 8 | [The Algorithm Design Manual](https://www.algorist.com/) | Steven Skiena | 3rd ed. |
| 9 | [Elements of Programming Interviews in Java](https://elementsofprogramminginterviews.com/) | Aziz, Lee & Prakash | Interview practice. A few problems a week keeps algorithms fresh |

---

## Phase 2 · Systems and Craft

**Course lane:** (CS50x on-ramp if needed) → 15-213 → 6.1810 → CS168.
**Book lane:** §6 → §7 (with the MIT 6.005 readings) → §8, in table order. Books #10–#13 are the companion texts for the courses.
**Milestone:** *A concurrent HTTP server on the JVM.* Go from raw sockets to HTTP/1.1 parsing, routing and static files, running on virtual threads. Write it test-first, load-test it, profile it with JDK Flight Recorder and async-profiler, and write up what you changed and why. The 15-213 malloc and proxy labs and the xv6 labs are this phase's systems milestones.

### 4 · Computer Systems and Operating Systems

| Course | Role | Materials |
|--------|------|-----------|
| [Harvard CS50x](https://cs50.harvard.edu/x/), weeks 1–5 | On-ramp | Only if C is new to you. Video · Notes · Problem sets with an autograder |
| [CMU 15-213 · Introduction to Computer Systems (Fall 2015)](https://www.cs.cmu.edu/afs/cs/academic/class/15213-f15/www/schedule.html) | Core | Video · Slides · [Self-study labs](http://csapp.cs.cmu.edu/3e/labs.html) · Practice problems with solutions in #10. C, x86-64 |
| [MIT 6.1810 · Operating System Engineering](https://pdos.csail.mit.edu/6.1810/) | Core | Video ([Fall 2020 lectures](https://pdos.csail.mit.edu/6.S081/2020/schedule.html)) · Notes and the xv6 book · Labs with a local grader · Quizzes + solutions. C, RISC-V |

| # | Title | Author(s) | Notes |
|---|-------|-----------|-------|
| 10 | [Computer Systems: A Programmer's Perspective](https://csapp.cs.cmu.edu/) | Bryant & O'Hallaron | 3rd ed. The 15-213 text |
| 11 | [Operating Systems: Three Easy Pieces](https://pages.cs.wisc.edu/~remzi/OSTEP/) | Remzi & Andrea Arpaci-Dusseau | Free online. The conceptual companion to 6.1810 |
| 12 | [The Linux Programming Interface](https://man7.org/tlpi/) | Michael Kerrisk | Reference |

---

### 5 · Networking

| Course | Role | Materials |
|--------|------|-----------|
| [UC Berkeley CS168 · Introduction to the Internet](https://cs168.io/) | Core | Notes ([free online textbook](https://textbook.cs168.io/)) · Projects · Past exams |
| [Kurose & Ross companion site](https://gaia.cs.umass.edu/kurose_ross/) | Core, with #13 | The authors' video lectures · Wireshark labs · Interactive problems |
| [Stanford CS144 · Introduction to Computer Networking](https://cs144.github.io/) | Deepen | Labs: build a working TCP implementation in C++, with test suites |

| # | Title | Author(s) | Notes |
|---|-------|-----------|-------|
| 13 | [Computer Networking: A Top-Down Approach](https://gaia.cs.umass.edu/kurose_ross/) | Kurose & Ross | |

---

### 6 · Concurrency and Performance

**Courses:** the theory comes from §4 (15-213 and 6.1810).

| Course | Role | Materials |
|--------|------|-----------|
| [MIT 6.172 · Performance Engineering of Software Systems (Fall 2018)](https://ocw.mit.edu/courses/6-172-performance-engineering-of-software-systems-fall-2018/) | Deepen | Video · Notes · Homework and projects · Quizzes + solutions. C |

| # | Title | Author(s) | Notes |
|---|-------|-----------|-------|
| 14 | [Java Concurrency in Practice](https://openlibrary.org/isbn/9780321349606) | Brian Goetz et al. | Read first: the memory model and the fundamentals the newer APIs build on |
| 15 | [Java Structured Concurrency](https://www.packtpub.com/en-us/product/java-structured-concurrency-9781806105021) | Anghel Leonard | Virtual threads, structured concurrency, scoped values |
| 16 | [Kotlin Coroutines Deep Dive](https://kt.academy/book/coroutines) | Marcin Moskała | |
| 17 | [Optimizing Cloud Native Java](https://www.oreilly.com/library/view/-/9781492039259/) | Evans, Gough & Newland | 2nd ed. |
| 18 | [Systems Performance](https://www.brendangregg.com/systems-performance-2nd-edition-book.html) | Brendan Gregg | 2nd ed. Reference |

---

### 7 · Software Design and Craftsmanship

| Course | Role | Materials |
|--------|------|-----------|
| [MIT 6.005 · Software Construction (Spring 2016)](https://ocw.mit.edu/courses/6-005-software-construction-spring-2016/) | Core | Readings · Problem sets. Java. No video: the readings are the lectures, and some of the best writing anywhere on specs, abstract data types, invariants and immutability |

| # | Title | Author(s) | Notes |
|---|-------|-----------|-------|
| 19 | [The Pragmatic Programmer](https://pragprog.com/titles/tpp20/the-pragmatic-programmer-20th-anniversary-edition/) | Hunt & Thomas | 20th anniversary ed. |
| 20 | [A Philosophy of Software Design](https://web.stanford.edu/~ouster/cgi-bin/book.php) | John Ousterhout | 2nd ed. Read before #21 |
| 21 | [Clean Code](https://openlibrary.org/isbn/9780132350884) | Robert C. Martin | Read critically, against #20 |
| 22 | [Refactoring](https://martinfowler.com/books/refactoring.html) | Martin Fowler | 2nd ed. |
| 23 | [Head First Design Patterns](https://openlibrary.org/isbn/9781492078005) | Freeman & Robson | 2nd ed. |
| 24 | [Working Effectively with Legacy Code](https://openlibrary.org/isbn/9780131177055) | Michael Feathers | |

---

### 8 · Testing

**Courses:** none. This topic is book-driven.

| # | Title | Author(s) | Notes |
|---|-------|-----------|-------|
| 25 | [Test-Driven Development by Example](https://openlibrary.org/isbn/9780321146533) | Kent Beck | |
| 26 | [Effective Software Testing](https://www.manning.com/books/effective-software-testing) | Mauricio Aniche | |
| 27 | [Unit Testing Principles, Practices, and Patterns](https://www.manning.com/books/unit-testing) | Vladimir Khorikov | |

---

## Phase 3 · Backend Engineering

**Course lane:** Spring Academy → 15-445 → CS161.
**Book lane:** §9 → §10 → §11, in table order.
**Milestone:** *A production-grade Spring Boot service.* Use a hexagonal structure (#29), REST with an OpenAPI contract plus one gRPC endpoint, and PostgreSQL with Flyway migrations. Tune JPA the way #36 teaches: no N+1 queries, deliberate fetch plans, batching. Add Testcontainers integration tests, an OAuth2 resource server with Spring Security, and metrics and traces. The 15-445 BusTub projects are this phase's systems milestone.

### 9 · Spring and APIs

| Course | Role | Materials |
|--------|------|-----------|
| [Spring Academy](https://spring.academy/) | Core | The official Spring courses: video lessons and hands-on labs. Use the [Spring guides](https://spring.io/guides) for each new Spring project you touch |

| # | Title | Author(s) | Notes |
|---|-------|-----------|-------|
| 28 | [Spring in Action](https://www.manning.com/books/spring-in-action-sixth-edition) | Craig Walls | 6th ed. Written for Spring Boot 2: learn the concepts here and the current APIs from the Spring docs |
| 29 | [Get Your Hands Dirty on Clean Architecture](https://reflectoring.io/book/) | Tom Hombergs | 2nd ed. Hexagonal architecture applied to a Spring service |
| 30 | [Modern API Development with Spring 6 and Spring Boot 3](https://www.packtpub.com/en-us/product/modern-api-development-with-spring-6-and-spring-boot-3-9781804613276) | Sourabh Sharma | |
| 31 | [API Design Patterns](https://www.manning.com/books/api-design-patterns) | J.J. Geewax | |
| 32 | [gRPC: Up and Running](https://openlibrary.org/isbn/9781492058335) | Indrasiri & Kuruppu | |
| 33 | [Pro Spring 6](https://link.springer.com/search?query=Pro+Spring+6+Schaefer) | Schaefer & Ho | Reference |
| 34 | [Reactive Spring](https://reactivespring.io/) | Josh Long | Optional. WebFlux, R2DBC, RSocket; pair with the Reactor and Spring reference docs. Virtual threads now cover most blocking-I/O scaling needs |

---

### 10 · Databases and Persistence

| Course | Role | Materials |
|--------|------|-----------|
| [CMU 15-445 · Database Systems](https://15445.courses.cs.cmu.edu/) | Core | Video ([CMU Database Group on YouTube](https://www.youtube.com/@CMUDatabaseGroup)) · Notes · Homework · Projects (BusTub, C++) · Exams + solutions |
| [CMU 15-721 · Advanced Database Systems](https://15721.courses.cs.cmu.edu/) | Deepen | Video · Paper readings |

| # | Title | Author(s) | Notes |
|---|-------|-----------|-------|
| 35 | [The Art of PostgreSQL](https://theartofpostgresql.com/) | Dimitri Fontaine | |
| 36 | [High-Performance Java Persistence](https://vladmihalcea.com/books/high-performance-java-persistence/) | Vlad Mihalcea | |
| 37 | [Database Internals](https://www.oreilly.com/library/view/-/9781492040330/) | Alex Petrov | Part I with 15-445; Part II with §12 |
| 38 | [Patterns of Enterprise Application Architecture](https://martinfowler.com/books/eaa.html) | Martin Fowler | Reference. The patterns JPA and Hibernate implement: Unit of Work, Identity Map, Data Mapper |

---

### 11 · Security

| Course | Role | Materials |
|--------|------|-----------|
| [UC Berkeley CS161 · Computer Security](https://cs161.org/) | Core | Notes ([free online textbook](https://textbook.cs161.org/)) · Projects · Exams + solutions |
| [Stanford CS253 · Web Security](https://web.stanford.edu/class/cs253/) | Deepen | Video (Fall 2019) · Slides · Assignments. The browser and HTTP side of backend security |
| [MIT 6.858 · Computer Systems Security (Fall 2014)](https://ocw.mit.edu/courses/6-858-computer-systems-security-fall-2014/) | Deepen | Video · Notes · Labs · Quizzes + solutions |

| # | Title | Author(s) | Notes |
|---|-------|-----------|-------|
| 39 | [Spring Security in Action](https://www.manning.com/books/spring-security-in-action-second-edition) | Laurențiu Spilcă | 2nd ed. |
| 40 | [OAuth 2 in Action](https://www.manning.com/books/oauth-2-in-action) | Richer & Sanso | |
| 41 | [Building Secure and Reliable Systems](https://sre.google/books/building-secure-reliable-systems/) | Adkins et al. (Google) | Free online |

---

## Phase 4 · Distributed Systems and Architecture

**Course lane:** Cambridge Distributed Systems → 6.5840 → Confluent courses.
**Book lane:** Understanding Distributed Systems → DDIA → Fundamentals of Software Architecture → Learning DDD → Building Microservices → Microservices Patterns → Kafka: The Definitive Guide → Building Event-Driven Microservices → The Hard Parts → Building Evolutionary Architectures. Read the rest of each section as your work calls for it.
**Milestone:** *Make it distributed.* The 6.5840 labs (MapReduce, Raft, a fault-tolerant key/value store) are the core milestone. Then split your Phase 3 service into two or three services along bounded contexts. Integrate them through Kafka with a transactional outbox and an orchestrated saga, make the consumers idempotent, and add consumer-driven contract tests.

### 12 · Distributed Systems

| Course | Role | Materials |
|--------|------|-----------|
| [Cambridge · Distributed Systems (Martin Kleppmann)](https://martin.kleppmann.com/2020/11/18/distributed-systems-and-elliptic-curves.html) | Core | Video (8 short lectures) · Notes with exercises · [Past exam questions](https://www.cl.cam.ac.uk/teaching/exams/pastpapers/). A short primer before 6.5840; pairs with #43 |
| [MIT 6.5840 · Distributed Systems](https://pdos.csail.mit.edu/6.824/) | Core | Video (2020 lectures) · Notes and papers · Labs with test suites · Exams + solutions. Go |
| [Fly.io · Gossip Glomers](https://fly.io/dist-sys/) | Deepen | Distributed-systems challenges you can solve in Java or Kotlin, checked by the Maelstrom harness |

| # | Title | Author(s) | Notes |
|---|-------|-----------|-------|
| 42 | [Understanding Distributed Systems](https://understandingdistributedsystems.com/) | Roberto Vitillo | Start here |
| 43 | [Designing Data-Intensive Applications](https://www.oreilly.com/library/view/designing-data-intensive-applications/9781098119058/) | Martin Kleppmann & Chris Riccomini | 2nd ed. (2026) |

---

### 13 · Software Architecture

| Course | Role | Materials |
|--------|------|-----------|
| [Mark Richards · Software Architecture Monday](https://www.developertoarchitecture.com/) | Deepen | Free short video lessons, one topic each. Pairs with #44 |

| # | Title | Author(s) | Notes |
|---|-------|-----------|-------|
| 44 | [Fundamentals of Software Architecture](https://openlibrary.org/search?q=Fundamentals+of+Software+Architecture+Richards+Ford) | Richards & Ford | 2nd ed. |
| 45 | [Software Architecture: The Hard Parts](https://openlibrary.org/search?q=Software+Architecture+The+Hard+Parts) | Ford, Richards, Sadalage & Dehghani | Read after §15 |
| 46 | [Building Evolutionary Architectures](https://evolutionaryarchitecture.com/) | Ford, Parsons, Kua & Sadalage | 2nd ed. Read last |

---

### 14 · Domain-Driven Design

**Courses:** none. This topic is book-driven.

| # | Title | Author(s) | Notes |
|---|-------|-----------|-------|
| 47 | [Learning Domain-Driven Design](https://www.oreilly.com/library/view/-/9781098100124/) | Vlad Khononov | Start here |
| 48 | [Implementing Domain-Driven Design](https://openlibrary.org/isbn/9780321834577) | Vaughn Vernon | |
| 49 | [Domain-Driven Design](https://www.domainlanguage.com/ddd/) | Eric Evans | Reference |

---

### 15 · Microservices

**Courses:** none. The distributed-systems theory is in §12; this section is about designing, building and running services.

| # | Title | Author(s) | Notes |
|---|-------|-----------|-------|
| 50 | [Building Microservices](https://samnewman.io/books/building_microservices_2nd_edition/) | Sam Newman | 2nd ed. |
| 51 | [Microservices Patterns](https://microservices.io/book) | Chris Richardson | |
| 52 | [Microservices with Spring Boot and Spring Cloud](https://openlibrary.org/search?q=Microservices+with+Spring+Boot+and+Spring+Cloud+Magnus+Larsson) | Magnus Larsson | |

---

### 16 · Event-Driven Systems and Streaming

| Course | Role | Materials |
|--------|------|-----------|
| [Confluent Developer · Kafka courses](https://developer.confluent.io/courses/) | Core | Video · Hands-on exercises. Start with Kafka 101 and Kafka Streams 101 |

| # | Title | Author(s) | Notes |
|---|-------|-----------|-------|
| 53 | [Enterprise Integration Patterns](https://www.enterpriseintegrationpatterns.com/) | Hohpe & Woolf | Reference. Read the opening chapters, then use the catalog |
| 54 | [Kafka: The Definitive Guide](https://www.confluent.io/resources/ebook/kafka-the-definitive-guide-v2/) | Shapira, Palino, Sivaram & Petty | 2nd ed.; free from Confluent |
| 55 | [Kafka Streams in Action](https://www.manning.com/books/kafka-streams-in-action-second-edition) | Bill Bejeck | 2nd ed. |
| 56 | [Building Event-Driven Microservices](https://www.oreilly.com/library/view/-/9781492057888/) | Adam Bellemare | |

---

## Phase 5 · Production and Staff-Level Practice

**Course lane:** DevOps with Docker → DevOps with Kubernetes → 6.033.
**Book lane:** §17 → §18 → §19, in table order.
**Milestone:** *Run it in production.* Ship the Phase 4 system to Kubernetes: container images, manifests (Helm or Kustomize), infrastructure as code, and a CI/CD pipeline with GitOps. Define SLOs with burn-rate alerts, and add dashboards and distributed traces through OpenTelemetry. Run a load test and a game-day failure exercise. Then write the design doc and a postmortem as if a staff-level review board were going to read them.

### 17 · Cloud Native, Delivery and Observability

| Course | Role | Materials |
|--------|------|-----------|
| [University of Helsinki · DevOps with Docker](https://devopswithdocker.com/) | Core | Text course · Exercises you submit for grading |
| [University of Helsinki · DevOps with Kubernetes](https://devopswithkubernetes.com/) | Core | Text course · Exercises you submit for grading. You build and run real apps on a cluster |

| # | Title | Author(s) | Notes |
|---|-------|-----------|-------|
| 57 | [Docker: Up & Running](https://www.oreilly.com/library/view/-/9781098131814/) | Kane & Matthias | 3rd ed. |
| 58 | [Kubernetes: Up & Running](https://www.oreilly.com/library/view/-/9781098110192/) | Burns, Beda, Hightower & Evenson | 3rd ed. |
| 59 | [Kubernetes Patterns](https://k8spatterns.io/) | Ibryam & Huß | 2nd ed. |
| 60 | [Continuous Delivery](https://continuousdelivery.com/) | Humble & Farley | |
| 61 | [Observability Engineering](https://www.oreilly.com/library/view/-/9781492076438/) | Majors, Fong-Jones & Miranda | |
| 62 | [AWS in Action](https://www.manning.com/books/amazon-web-services-in-action-third-edition) | Michael & Andreas Wittig | 3rd ed. |

---

### 18 · Reliability and System Design

| Course | Role | Materials |
|--------|------|-----------|
| [MIT 6.033 · Computer System Engineering (Spring 2018)](https://ocw.mit.edu/courses/6-033-computer-system-engineering-spring-2018/) | Core | Video · Classic systems papers · Quizzes + solutions · Design project. Now numbered 6.1800. At this stage the value is the design project and the writing |

| # | Title | Author(s) | Notes |
|---|-------|-----------|-------|
| 63 | [Release It!](https://pragprog.com/titles/mnee2/release-it-second-edition/) | Michael Nygard | 2nd ed. |
| 64 | [Site Reliability Engineering](https://sre.google/sre-book/table-of-contents/) | Beyer et al. (Google) | Free online. Pair with [The Site Reliability Workbook](https://sre.google/workbook/table-of-contents/) (also free) for SLO practice |
| 65 | [System Design Interview: Volume 1](https://bytebytego.com/) | Alex Xu | Interview prep |
| 66 | [System Design Interview: Volume 2](https://bytebytego.com/) | Alex Xu & Sahn Lam | Interview prep |

---

### 19 · Engineering Practice and Staff-Level Leadership

**Courses:** none. This topic is book-driven.

| # | Title | Author(s) | Notes |
|---|-------|-----------|-------|
| 67 | [Software Engineering at Google](https://abseil.io/resources/swe-book) | Winters, Manshreck & Wright | Free online |
| 68 | [The Staff Engineer's Path](https://www.oreilly.com/library/view/-/9781098118723/) | Tanya Reilly | |
| 69 | [Accelerate](https://itrevolution.com/product/accelerate/) | Forsgren, Humble & Kim | Optional |

---

*Memento Mori. Memento Vivere.*
