# Quang Minh

Software Engineering student building reliable web and mobile products with Django, Next.js, React Native, and PostgreSQL.

I care about the parts that make a product survive beyond a demo: explicit API contracts, authorization boundaries, concurrent state, recovery after lost connections, tests, and a verifiable release process.

[View GoPlan](https://github.com/theartroutine/GoPlan)

## Featured project — GoPlan

**GoPlan** is a full-stack group trip planning and coordination platform. It keeps itinerary planning, shared expenses, realtime chat, photos, memory videos, and an AI trip assistant under one trip permission model.

[![GoPlan dashboard](https://raw.githubusercontent.com/theartroutine/GoPlan/main/.github/assets/readme/screenshots/dashboard.webp)](https://github.com/theartroutine/GoPlan)

### What is technically interesting

- **Web architecture:** Next.js Backend-for-Frontend in front of a Django REST API; refresh tokens stay in httpOnly cookies and access tokens stay in memory.
- **Realtime reliability:** Django Channels, Redis, ticket-authenticated WebSockets, monotonic event ordering, reconnect handling, and session-bound ownership.
- **Money workflows:** shared trip expenses, contribution tracking, settlement calculation, and sent/received transfer confirmation.
- **Human-in-the-loop AI:** GoPlanAI can read trip context and propose actions, but mutations remain drafts until an authorized user confirms them.
- **Media pipeline:** optimized photo uploads and background FFmpeg rendering for shareable trip highlight videos.
- **Multiple clients:** a Next.js web application and an Expo/React Native mobile application share the Django domain contracts.
- **Verification:** extensive backend, frontend, and mobile test suites cover permissions, concurrency, API contracts, realtime recovery, money calculations, and AI draft behavior.

**Stack:** Django 5.2 · Django REST Framework · Next.js 16 · React 19 · Expo/React Native · TypeScript · PostgreSQL · Redis · Celery · Podman · FFmpeg

## How I work

1. Turn a product request into an explicit contract and acceptance criteria.
2. Trace the change across domain, API, client state, security, and failure modes.
3. Implement in reviewable slices with regression coverage.
4. Verify static checks and the rendered/runtime journey separately.
5. Record what was proven, what remains unverified, and the operational risks.

I use coding agents as implementation leverage, while retaining responsibility for scope, architecture, review, testing, and release decisions. Generated code is a draft until it survives the same review and verification gates as any other contribution.

## Areas I can help with

- Django/DRF APIs and service-layer business logic
- Next.js BFF integrations and authenticated application flows
- WebSocket/realtime state, reconnection, ordering, and idempotency bugs
- Expo/React Native feature work and native iOS Simulator QA
- Focused debugging, regression tests, and implementation review

I am open to scoped remote collaboration where the expected outcome can be defined and verified clearly.
