U<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:050816,45:0B1F3A,100:00D9FF&height=200&section=header&text=SUBHAMOY%20DATTA&fontSize=44&fontColor=E6F7FF&fontAlignY=35&animation=fadeIn&desc=GENAI%20BACKEND%20ENGINEER%20%7C%20RAG%20SYSTEMS%20%7C%20AI%20AGENTS&descAlignY=57&descSize=16"/>

<a href="https://github.com/subhamoydatta703">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=19&duration=2600&pause=900&color=00D9FF&center=true&vCenter=true&repeat=true&width=760&height=55&lines=Building+production-grade+GenAI+backend+systems.;Designing+RAG+pipelines+for+grounded+retrieval.;Engineering+transparent+AI+agent+systems.;Focused+on+backend+and+AI+infrastructure." alt="Animated typing headline"/>
</a>

<br/>



</div>

<div align="center">

```bash
subhamoy@dev:~$ whoami
subhamoydatta703

subhamoy@dev:~$ cat role.txt
GenAI Backend Engineer — RAG Systems & Agent Architecture

subhamoy@dev:~$ cat status.txt
B.Tech CSE (AI & ML) — building backend + AI systems in parallel

subhamoy@dev:~$ _
```

</div>

## Focus Areas

**Building**
REST APIs, backend architecture, RAG pipelines, vector search, background job systems, authentication and authorization, cloud-integrated services, agentic workflows.

**Sharpening**
Data Structures & Algorithms, Low-Level Design, Advanced SQL, backend system design, DevOps fundamentals.

**Exploring next**
Multi-agent orchestration, retrieval evaluation, distributed job queues at scale.

## Somoy — Agent SDK

<div align="center">

<a href="https://www.npmjs.com/package/@subhamoy/somoy">
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=20&duration=2800&pause=1000&color=00D9FF&center=true&vCenter=true&repeat=true&width=760&height=48&lines=%40subhamoy%2Fsomoy;Transparent%2C+Hand-Written+Agent+SDK;Plan+%E2%86%92+Act+%E2%86%92+Observe%2C+Fully+Inspectable;One+Interface.+Three+Providers.;No+Framework+Opinions%2C+No+Hidden+Retries" alt="Somoy animated title"/>
</a>

</div>

A transparent AI agent SDK for TypeScript, built around an explicit, inspectable `plan → act → observe` execution loop. No hidden state, no framework abstraction standing between the developer and what the agent is actually doing. Most agent frameworks ask you to inherit a large stack of opinions before you can see a single line of the loop — Somoy makes the opposite bet: a small, provider-agnostic runtime that a TypeScript developer can fully read and modify in an afternoon.

**What sets it apart**
The entire loop is one explicit, hand-written state machine, so every exit path can be traced and breakpointed directly. A single `ModelProvider` interface backs three interchangeable adapters — Gemini, OpenAI, and an offline Mock — so switching providers is a one-line change with nothing else in the agent touched. Failures are typed values rather than thrown exceptions: loop detection, handoff ping-pong, guardrail rejections, timeouts, and model errors all resolve to a `RunResult` carrying a status discriminant, so expected failure modes never need a try/catch.

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=15&duration=1800&pause=500&color=00D9FF&center=true&vCenter=true&repeat=true&width=700&height=100&lines=MODEL+selects+Gemini+%2F+OpenAI+%2F+Mock;PLAN+%E2%86%92+structured+output;ACT+%E2%86%92+execute+tools;OBSERVE+%E2%86%92+read+tool+results;done+%E2%86%92+typed+RunResult" alt="Animated plan-act-observe loop"/>

</div>

<div align="center">

| Capability | Implementation |
|---|---|
| Model providers | Gemini · OpenAI · Offline Mock |
| Type safety | TypeScript + Zod |
| Tool execution | Typed tool inputs / outputs |
| Structured outputs | Zod-inferred schemas |
| Failure handling | Typed `RunResult` values |
| Multi-agent | Transcript handoffs, ping-pong prevention |
| Reliability | Retries · backoff · timeouts · loop detection |
| Persistence | In-memory + SQLite |
| Runtime | Bun · Node.js 18+ |

</div>

<div align="center">

<a href="https://www.npmjs.com/package/@subhamoy/somoy">
<img src="https://img.shields.io/npm/v/@subhamoy/somoy?style=for-the-badge&logo=npm&logoColor=white&color=00D9FF" />
</a>
<a href="https://github.com/subhamoydatta703/Agent-SDK">
<img src="https://img.shields.io/badge/SOURCE-0B1F3A?style=for-the-badge&logo=github&logoColor=FFFFFF" />
</a>

</div>

## Selected Builds

**DocSense**

RAG-powered document intelligence platform for ingesting documents and knowledge sources and answering questions with grounded, source-backed responses.

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=14&duration=1900&pause=500&color=00D9FF&center=true&vCenter=true&repeat=true&width=700&height=90&lines=INGEST%3A+PDF+%C2%B7+URL+%C2%B7+YouTube+%C2%B7+Text;PROCESS+%E2%86%92+CHUNK+%E2%86%92+EMBED;pgvector+semantic+search;Grounded+response+with+sources" alt="Animated DocSense pipeline"/>
</p>

Documents, web pages, YouTube transcripts, and raw text are chunked and embedded into PostgreSQL via pgvector. Before a query reaches the retriever, it passes through a step-back optimization stage that pulls broader, more relevant context instead of surface-level matches. Ingestion runs asynchronously through BullMQ and Redis, backed by rate limiting, input/output guardrails, and Clerk-based authentication.

*Stack* — React · TypeScript · Bun · Express · PostgreSQL · pgvector · Redis · BullMQ · AWS S3 · Gemini API · Clerk

<p align="center">
  <a href="https://docsense-app.vercel.app">
    <img src="https://img.shields.io/badge/LIVE%20DEMO-00D9FF?style=for-the-badge&logo=vercel&logoColor=050816" />
  </a>
  <a href="https://github.com/subhamoydatta703/DocSense">
    <img src="https://img.shields.io/badge/SOURCE-0B1F3A?style=for-the-badge&logo=github&logoColor=FFFFFF" />
  </a>
</p>

**Resumark**

AI-powered resume analysis platform with asynchronous processing, caching, and production-ready backend infrastructure.

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=14&duration=1900&pause=500&color=00D9FF&center=true&vCenter=true&repeat=true&width=700&height=90&lines=PDF+%E2%86%92+PARSE+%E2%86%92+QUEUE;AI+ANALYSIS%3A+ATS+%C2%B7+Skills+%C2%B7+Summary+%C2%B7+Formatting;Redis+%2B+Postgres+cache;Report+delivered" alt="Animated Resumark pipeline"/>
</p>

A resume is parsed, queued for analysis, and returned with an ATS score, skills breakdown, summary, and formatting feedback — generated by Gemini and run through a background job pipeline rather than a blocking API call. Results are cached in Redis and backed by Postgres, with resumes stored in AWS S3, so repeat runs stay fast under load.

*Stack* — Bun · TypeScript · Express · PostgreSQL · Prisma · Redis · BullMQ · AWS S3 · Gemini API

<p align="center">
  <a href="https://resumark-webapp.vercel.app">
    <img src="https://img.shields.io/badge/LIVE%20DEMO-00D9FF?style=for-the-badge&logo=vercel&logoColor=050816" />
  </a>
  <a href="https://github.com/subhamoydatta703/Resumark">
    <img src="https://img.shields.io/badge/SOURCE-0B1F3A?style=for-the-badge&logo=github&logoColor=FFFFFF" />
  </a>
</p>

**ShelfLife**

Full-stack household inventory and expiry-tracking application for shared household management.

Households form around a simple invite code, and every member sees the same inventory with expiry status derived automatically — fresh, expiring soon, or already gone. Items are marked used or wasted as they're consumed, and JWT-based auth scopes each household's data to the people actually in it, with expiry notifications nudging users before food goes bad.

*Stack* — React · Node.js · Express · MongoDB · JWT

<p align="center">
  <a href="https://shelf-life-webapp.vercel.app">
    <img src="https://img.shields.io/badge/LIVE%20DEMO-00D9FF?style=for-the-badge&logo=vercel&logoColor=050816" />
  </a>
  <a href="https://github.com/subhamoydatta703/Shelf-Life">
    <img src="https://img.shields.io/badge/SOURCE-0B1F3A?style=for-the-badge&logo=github&logoColor=FFFFFF" />
  </a>
</p>

## Toolkit

<div align="center">

<img src="https://skillicons.dev/icons?i=typescript,javascript,java,python,nodejs,bun,express,react,nextjs,tailwind,postgres,mongodb,prisma,redis,docker,aws,linux,git,github,vscode&theme=dark" />

<br/><br/>

<img src="https://img.shields.io/badge/pgvector-00D9FF?style=for-the-badge" />
<img src="https://img.shields.io/badge/BullMQ-EA4335?style=for-the-badge" />
<img src="https://img.shields.io/badge/AWS_S3-FF9900?style=for-the-badge" />
<img src="https://img.shields.io/badge/Clerk-6C47FF?style=for-the-badge" />
<img src="https://img.shields.io/badge/Gemini_AI-4285F4?style=for-the-badge" />
<img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge" />
<img src="https://img.shields.io/badge/Render-46E3B7?style=for-the-badge" />

</div>

## Skill Matrix

<div align="center">

| Domain | Skills |
|---|---|
| Backend | REST APIs, backend architecture, API design, authentication, authorization, background jobs, rate limiting, file uploads |
| AI / GenAI | Gemini API, RAG pipelines, vector search, AI agents, agent SDK design, prompt engineering, structured outputs, Zod |
| Data | PostgreSQL, pgvector, MongoDB, Prisma, Redis |
| Infrastructure | Docker, AWS, Render, Vercel, Bun, Express |

</div>

## Activity Log

<div align="center">

<img src="https://ghchart.rshah.org/00D9FF/subhamoydatta703" width="100%" alt="GitHub contribution graph"/>

<br/><br/>

<img height="180" src="https://awesome-github-stats.azurewebsites.net/user-stats/subhamoydatta703?cardType=level-alternate&theme=dark&fontFamily=42dot%20Sans&preferLogin=false" />



</div>

## Elsewhere

<div align="center">

<a href="https://github.com/subhamoydatta703">
<img src="https://img.shields.io/badge/GITHUB-SUBHAMOYDATTA703-0B1F3A?style=for-the-badge&logo=github&logoColor=00D9FF" />
</a>
<a href="https://www.linkedin.com/in/subhamoy-datta">
<img src="https://img.shields.io/badge/LINKEDIN-SUBHAMOY%20DATTA-0B1F3A?style=for-the-badge&logo=linkedin&logoColor=00D9FF" />
</a>
<a href="https://x.com/itssubhamoy">
<img src="https://img.shields.io/badge/X-SUBHAMOY-0B1F3A?style=for-the-badge&logo=x&logoColor=00D9FF" />
</a>
<a href="mailto:subhamoydatta703@gmail.com">
<img src="https://img.shields.io/badge/GMAIL-SUBHAMOYDATTA703-0B1F3A?style=for-the-badge&logo=gmail&logoColor=00D9FF" />
</a>

<br/><br/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=16&duration=3000&pause=1200&color=00D9FF&center=true&vCenter=true&repeat=true&width=720&height=42&lines=Build+%E2%86%92+Break+%E2%86%92+Learn+%E2%86%92+Rebuild;Backend+%2B+RAG+%2B+Agents" alt="Closing animation"/>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:050816,45:0B1F3A,100:00D9FF&height=110&section=footer&animation=fadeIn"/>

</div>
