Act as a Principal Full-Stack Architect, Senior Next.js Engineer, Senior NestJS Engineer, PostgreSQL/Prisma Database Architect, 3D Web Experience Designer, UI/UX Product Designer, DevOps Engineer, Security Engineer, Accessibility Specialist, Performance Engineer, and QA Automation Engineer.

Your task is to CREATE FROM SCRATCH a complete, production-ready, visually extraordinary Habit, Goal, Routine, Focus, and Productivity Tracking platform.

Do not create only a design, prototype, landing page, or dashboard mockup.

BUILD THE ACTUAL FULL-STACK APPLICATION AND WRITE THE COMPLETE WORKING CODEBASE.

============================================================
PRODUCT
============================================================

Product working name:

MOMENTUM

Tagline:

BUILD BETTER DAYS.
BECOME BETTER EVERY DAY.

The objective is to create a world-class habit-tracking experience with:

• Premium 3D animated landing page
• Glassmorphism / glass UI
• Powerful habit tracking
• Goal + milestone management
• Routine management
• Focus timer
• Advanced analytics
• Streaks
• Heatmaps
• Gamification
• Beautiful responsive dashboards
• Offline capability
• PWA support
• Secure authentication
• Production backend
• PostgreSQL
• Redis
• Observability
• Docker
• CI/CD

The application must work exceptionally well on:

📱 Mobile
📱 Tablet
💻 Laptop
🖥 Desktop
📲 Installable PWA

Do NOT simply scale down the desktop interface for mobile.

Create intentionally designed mobile and desktop experiences.

============================================================
1. MANDATORY TECHNOLOGY STACK
============================================================

Use this architecture unless there is a genuine technical incompatibility.

WEB FRONTEND
Next.js + React + TypeScript

BACKEND
NestJS + TypeScript

DATABASE
PostgreSQL

ORM
Prisma

CACHE
Redis

OFFLINE LOCAL STORAGE
SQLite where technically appropriate for the target runtime.

IMPORTANT:
For browser/PWA offline persistence, do not force server-style SQLite into an environment where it is inappropriate.

Use a browser-compatible persistence layer such as IndexedDB where necessary while preserving a repository/storage abstraction that can support SQLite for native/local runtimes.

Explain this implementation decision in the architecture documentation.

STYLING
Tailwind CSS

NativeWind should be reserved for a future/actual React Native client where applicable. Do not unnecessarily force NativeWind into normal Next.js DOM components.

SERVER STATE
TanStack Query

CLIENT/UI STATE
Zustand

VALIDATION
Zod

API
REST

API DOCUMENTATION
OpenAPI / Swagger

CONTAINERS
Docker

CI/CD
GitHub Actions

CACHE / SESSION / RATE-LIMITING SUPPORT
Redis

OBSERVABILITY
OpenTelemetry

METRICS
Prometheus

DASHBOARDS
Grafana

============================================================
2. MONOREPO ARCHITECTURE
============================================================

Create a professional monorepo.

Suggested architecture:

apps/
    web/
    api/

packages/
    ui/
    types/
    validation/
    config/
    api-client/
    eslint-config/
    tsconfig/
    observability/

prisma/

docker/

monitoring/

.github/
    workflows/

docs/

Use pnpm workspaces or another strong monorepo solution.

Avoid duplicated types and validation schemas wherever practical.

============================================================
3. ENGINEERING STANDARDS
============================================================

Use:

• TypeScript strict mode
• Server Components where beneficial
• Client Components only when required
• Proper DTO architecture
• Dependency injection
• Repository/service patterns where useful
• Modular NestJS architecture
• Shared Zod schemas where appropriate
• ESLint
• Prettier
• Environment validation
• Database migrations
• Database seeding
• Unit tests
• Integration tests
• E2E tests
• Structured logging
• Error boundaries
• Loading states
• Empty states

Do NOT create giant files or giant React components.

Separate business logic from presentation.

============================================================
4. 3D VISUAL EXPERIENCE
============================================================

This is one of the application's defining features.

Create a premium 3D experience using technologies appropriate for React such as:

• Three.js
• React Three Fiber
• Drei
• Framer Motion / Motion
• CSS transforms
• GPU-friendly effects

Do not add 3D merely for decoration.

Use it strategically to communicate:

PROGRESS
MOMENTUM
GROWTH
CONSISTENCY
ACHIEVEMENT

============================================================
5. 3D LANDING PAGE
============================================================

Build an exceptional animated landing page.

The first screen should immediately look like a premium technology product.

Create an immersive hero.

LEFT:

Large headline:

BUILD BETTER
HABITS.

Smaller animated gradient/glass text:

BECOME BETTER
EVERY DAY.

Description:

Build consistency, achieve meaningful goals, understand your progress, and turn small daily actions into lasting results.

Primary CTA:

START BUILDING

Secondary CTA:

EXPLORE FEATURES

RIGHT:

Create an interactive 3D visualization.

Possible concept:

A floating translucent 3D progress sphere/orb surrounded by habit rings.

Each orbit represents:

Health
Learning
Fitness
Career
Mindfulness
Productivity

The orb should react subtly to:

• Mouse movement
• Pointer movement
• Scroll
• Completion progress

Use particles or subtle ambient elements around it.

Do NOT make the scene visually overwhelming.

============================================================
6. LANDING PAGE SCROLL STORY
============================================================

Create an immersive scrolling experience.

Sections:

01 — HERO

02 — BUILD CONSISTENCY

03 — TRACK EVERYTHING

04 — STREAKS

05 — GOALS

06 — ROUTINES

07 — ANALYTICS

08 — FOCUS

09 — HEATMAP

10 — PRODUCT SHOWCASE

11 — MOBILE EXPERIENCE

12 — SECURITY / PRIVACY

13 — FINAL CTA

Use smooth transitions between sections.

Possible effects:

• 3D object transformations
• Glass cards entering depth
• Number counters
• Progress rings filling
• Charts animating
• Floating UI cards
• Perspective transforms
• Scroll-linked movement
• Parallax
• Subtle particles

Animations must remain smooth and performant.

============================================================
7. GLASSMORPHISM DESIGN SYSTEM
============================================================

Create an original premium glass UI.

Use:

• Translucent surfaces
• Background blur
• Thin luminous borders
• Layered depth
• Soft shadows
• Gradient lighting
• Subtle reflections
• Large rounded corners
• Spacious layouts

Do not apply extreme blur everywhere.

Glass effects must maintain readability.

Example design tokens:

Background:
deep navy / near-black

Surface:
semi-transparent neutral glass

Primary:
electric blue / cyan

Secondary:
violet

Success:
bright accessible green

Warning:
amber

Danger:
coral/red

Text:
near-white in dark mode

============================================================
8. LIGHT + DARK MODE
============================================================

Create both.

LIGHT MODE

Clean
Bright
Premium
Minimal

DARK MODE

Deep
Atmospheric
Glass-heavy
Immersive

Support:

• System theme
• Manual selection
• Persistent preference

All charts and 3D elements must adapt.

============================================================
9. ACCESSIBILITY
============================================================

Target WCAG 2.2 AA.

Implement:

• Semantic HTML
• Keyboard navigation
• Screen-reader labels
• Proper focus indicators
• Accessible forms
• High contrast
• ARIA only where necessary
• Large touch targets
• Reduced-motion support

CRITICAL:

If prefers-reduced-motion is enabled:

Reduce or disable:

• Parallax
• Continuous rotation
• Large transitions
• Particle effects

Provide useful static alternatives to important 3D content.

============================================================
10. PERFORMANCE-AWARE 3D
============================================================

3D must never destroy application performance.

Implement:

• Dynamic loading
• Lazy loading
• Suspense
• Code splitting
• Adaptive DPR
• Reduced particle count on mobile
• GPU-friendly animation
• IntersectionObserver
• Pause animations when offscreen
• Reduced effects on low-powered devices

Do not load the full 3D landing experience inside the authenticated dashboard unless required.

============================================================
11. LOGIN PAGE
============================================================

Create a premium dedicated authentication experience.

Desktop:

Use a split layout.

LEFT:
Interactive visual/3D experience.

RIGHT:
Floating glass login card.

Mobile:
Simplified high-performance animated background with centered authentication card.

Login card:

MOMENTUM

WELCOME BACK

Continue building a better version of yourself.

Fields:

Email
Password

Actions:

LOGIN

CONTINUE WITH GOOGLE

Forgot Password?

Don't have an account?
CREATE ACCOUNT

Include:

• Password visibility toggle
• Remember me
• Loading state
• Error state
• Form validation
• Keyboard support
• Mobile optimization

============================================================
12. REGISTRATION
============================================================

Fields:

Name
Email
Password
Confirm Password

Include:

CREATE ACCOUNT

CONTINUE WITH GOOGLE

Password requirements should be clearly displayed.

After successful registration, start onboarding.

============================================================
13. AUTHENTICATION
============================================================

Implement secure authentication.

Support:

• Email/password
• Google OAuth
• Email verification
• Forgot password
• Reset password
• Logout
• Refresh/session lifecycle
• Session revocation

Use secure HTTP-only cookies where appropriate.

Never store sensitive auth tokens insecurely in localStorage.

============================================================
14. AUTH SECURITY
============================================================

Implement:

• Strong password hashing
• Secure cookies
• SameSite configuration
• HTTPS production assumptions
• CSRF protection where applicable
• Rate limiting
• Brute-force protection
• Input validation
• OAuth state/PKCE where appropriate
• Secure logout
• Secret management

Never commit secrets.

============================================================
15. ONBOARDING EXPERIENCE
============================================================

Create a beautiful multi-step onboarding flow.

STEP 1
Welcome

STEP 2
What would you like to improve?

Options:

Health
Fitness
Productivity
Learning
Career
Mindfulness
Sleep
Finance

STEP 3
Select starter habits.

STEP 4
Choose goals.

STEP 5
Set reminder preferences.

STEP 6
Choose theme.

STEP 7
Personalize dashboard.

Use progress indicators.

Allow users to skip optional steps.

============================================================
16. APPLICATION SHELL
============================================================

Desktop navigation:

Dashboard
Today
Habits
Calendar
Routines
Goals
Focus
Analytics
Reviews
Achievements
Settings

Use a collapsible glass sidebar.

Mobile bottom navigation:

🏠 Home
✅ Habits
🎯 Goals
📊 Insights
☰ More

Provide a floating + action button.

============================================================
17. MAIN DASHBOARD
============================================================

Create a premium personalized dashboard.

Header:

Good Morning, [Name]

Today's date

Motivational message

Primary progress card:

TODAY'S PROGRESS

Example:

78%

7 / 9 HABITS

Additional KPI cards:

🔥 Current Streak

🏆 Longest Streak

🎯 Active Goals

⏱ Focus Time

📈 Weekly Progress

⭐ Consistency Score

============================================================
18. 3D PROGRESS VISUALIZATION
============================================================

Create an optional interactive progress visualization.

For example:

A circular 3D habit universe.

Completed habits become illuminated.

Incomplete habits remain translucent.

As users complete habits:

• Progress ring fills
• Orb illumination increases
• Small particle celebration occurs
• Percentage updates

Do not make completion depend on the 3D interface.

Always provide accessible standard controls.

============================================================
19. TODAY PAGE
============================================================

Show:

Today's habits
Today's routines
Upcoming milestones
Focus sessions
Today's notes

Each habit card:

Icon
Name
Category
Target
Current streak
Progress
Complete button

Completion must be possible with one click/tap.

Provide Undo.

============================================================
20. HABIT MANAGEMENT
============================================================

Users can:

Create
Edit
Pause
Resume
Archive
Delete

Fields:

Name
Description
Icon
Category
Color
Frequency
Target
Unit
Priority
Start Date
Optional End Date
Reminder
Status

============================================================
21. HABIT SCHEDULES
============================================================

Support:

Daily

Weekdays

Weekends

Specific weekdays

X times/week

X times/month

Custom schedule

Calculations must respect schedules.

Never penalize users for days when a habit was not scheduled.

============================================================
22. HABIT LOGGING
============================================================

Store historical logs.

A habit log should support:

Date
Completed status
Numeric value where applicable
Notes
Completion timestamp

Examples:

Drink Water
2.5 / 3 L

Read
45 / 60 minutes

Workout
Completed

============================================================
23. STREAK ENGINE
============================================================

Implement accurate streak calculations.

Track:

Current streak
Longest streak
Total completions
Missed scheduled days
Completion %
Consistency score

Milestones:

🔥 3 Days
🔥 7 Days
🏆 14 Days
🏆 30 Days
💎 60 Days
👑 100 Days
🚀 365 Days

============================================================
24. HABIT CALENDAR
============================================================

Create:

Day
Week
Month

views.

Users should be able to click a date and inspect:

Completed habits
Missed habits
Routine activity
Focus sessions
Goal activity
Notes

============================================================
25. HABIT HEATMAP
============================================================

Build a GitHub-style heatmap.

Filters:

Last Month
3 Months
6 Months
1 Year

Hover/tap:

Date
Completion %
Completed
Scheduled

============================================================
26. ROUTINES
============================================================

Users can create:

Morning Routine
Evening Routine
Study Routine
Work Routine
Workout Routine
Custom Routine

Each routine contains ordered steps.

Support drag-and-drop ordering.

Fields:

Routine name
Schedule
Time
Activities
Reminder
Status

============================================================
27. FOCUS SYSTEM
============================================================

Create a premium focus timer.

Modes:

25 / 5 Pomodoro

50 / 10

Custom

Display:

Timer
Task
Category
Session progress
Today's focus total

Track:

Duration
Completed session
Date
Task
Category

============================================================
28. GOALS
============================================================

Goal fields:

Name
Description
Category
Priority
Start Date
Target Date
Status
Progress
Notes

Users can:

Create
Edit
Archive
Complete
Delete

============================================================
29. GOAL MILESTONES
============================================================

Goals can contain milestones.

Example:

GOAL:
Become Job Ready

MILESTONES:

✓ Finish course
✓ Build portfolio
○ Build three projects
○ Update resume
○ Complete mock interviews

Calculate goal progress automatically.

============================================================
30. GOAL DEADLINES
============================================================

Show:

✓ Completed

⏳ 14 Days Left

⚠ Due Soon

🚨 Overdue

Create upcoming deadline widgets.

============================================================
31. WEEKLY REVIEW
============================================================

Ask:

What went well?

What was difficult?

Which habit performed best?

Which habit needs attention?

What distracted you?

What was your biggest win?

What will you improve?

What is next week's main focus?

Weekly Rating:
1–5 stars

Store historical reviews.

============================================================
32. ANALYTICS
============================================================

Create a dedicated analytics experience.

Sections:

Overview
Habits
Goals
Focus
Categories
Trends

============================================================
33. WEEKLY ANALYTICS
============================================================

Display:

Weekly completion
Completed activities
Missed activities
Best habit
Weakest habit
Best day
Current streak
Focus time

Compare:

THIS WEEK
VS
LAST WEEK

Show percentage difference.

============================================================
34. MONTHLY ANALYTICS
============================================================

Show:

Overall completion
Completed activities
Missed activities
Best habit
Weakest habit
Best day
Best week
Current streak
Longest streak
Goal completion
Focus time
Category performance

============================================================
35. YEARLY ANALYTICS
============================================================

Display:

January → December

Show:

Monthly completion
Annual average
Goals completed
Best month
Weakest month
Longest streak
Total focus hours
Consistency score

============================================================
36. CHARTS
============================================================

Create beautiful responsive charts.

Include:

Line charts
Area charts
Bar charts
Donut charts
Progress rings
Heatmaps

Every chart should have:

Tooltips
Labels where appropriate
Accessible summaries
Loading states
Empty states

============================================================
37. SMART INSIGHTS
============================================================

Create rule-based insights without requiring paid AI.

Examples:

"You improved by 12% compared with last week."

"Tuesday is your most productive day."

"Workout is currently your strongest habit."

"Reading has been missed three times this week."

"You're two days away from matching your longest streak."

============================================================
38. ACHIEVEMENTS
============================================================

Create tasteful gamification.

Achievements:

First Habit
First Goal
3-Day Streak
7-Day Streak
30-Day Streak
100 Completions
10 Focus Hours
First Perfect Week
First Goal Completed

Create premium achievement cards.

Avoid childish gamification.

============================================================
39. NOTIFICATIONS
============================================================

Support:

Habit reminders
Routine reminders
Goal reminders
Milestone reminders
Weekly review reminders
Streak warnings

Allow granular notification controls.

============================================================
40. PWA
============================================================

Make the Next.js application installable.

Implement:

Web App Manifest
Service Worker strategy
App icons
Install experience
Offline fallback
Caching strategy

Where feasible:

Allow offline habit completion.

Queue mutations locally.

Sync when connectivity returns.

Prevent duplicate synchronization.

============================================================
41. DATABASE
============================================================

Use PostgreSQL + Prisma.

Design normalized entities including:

User
Account
Session
UserPreference

Habit
HabitSchedule
HabitLog

Routine
RoutineItem
RoutineLog

Goal
Milestone

FocusSession

WeeklyReview

Achievement
UserAchievement

Reminder
NotificationPreference

AuditEvent where appropriate

============================================================
42. DATABASE INTEGRITY
============================================================

Use:

Primary keys
Foreign keys
Unique constraints
Indexes
Created timestamps
Updated timestamps
Soft deletion where beneficial

Important indexes should cover common queries such as:

user + date

habit + date

user + status

goal + target date

============================================================
43. PRISMA
============================================================

Provide:

schema.prisma

Migrations

Seed script

Development sample data

Production-safe configuration

============================================================
44. REDIS
============================================================

Use Redis strategically.

Possible uses:

Caching
Rate limiting
Short-lived state
Distributed locks
Idempotency
Background-job support

Do not cache everything blindly.

Document cache invalidation.

============================================================
45. NESTJS BACKEND
============================================================

Create modular NestJS modules such as:

AuthModule
UsersModule
HabitsModule
HabitLogsModule
RoutinesModule
GoalsModule
FocusModule
AnalyticsModule
ReviewsModule
AchievementsModule
NotificationsModule
HealthModule
ObservabilityModule

Use:

Controllers
Services
DTOs
Guards
Interceptors
Filters
Pipes

============================================================
46. REST API
============================================================

Create versioned APIs.

Example:

/api/v1/auth

/api/v1/users

/api/v1/habits

/api/v1/habit-logs

/api/v1/routines

/api/v1/goals

/api/v1/focus

/api/v1/reviews

/api/v1/analytics

/api/v1/achievements

/api/v1/settings

Use correct HTTP semantics.

============================================================
47. OPENAPI
============================================================

Generate Swagger/OpenAPI documentation.

Include:

Schemas
Request examples
Response examples
Authentication requirements
Error responses
Validation

Expose development Swagger UI.

============================================================
48. ZOD
============================================================

Use Zod for frontend/form/domain validation where appropriate.

Avoid contradictory frontend/backend validation rules.

Share validation schemas where architecture allows.

============================================================
49. TANSTACK QUERY
============================================================

Use TanStack Query for:

Fetching
Caching
Mutation
Optimistic updates
Invalidation
Retry logic

Habit completion should feel instant using optimistic UI where safe.

============================================================
50. ZUSTAND
============================================================

Use Zustand only for appropriate client state such as:

UI preferences
Sidebar state
Modal state
Temporary timer state
Theme-related application state

Do not duplicate server data unnecessarily inside Zustand.

============================================================
51. OFFLINE DATA ARCHITECTURE
============================================================

Create an offline abstraction.

The user requested SQLite.

Use SQLite for runtimes where SQLite is technically appropriate.

For browser PWA offline persistence, use IndexedDB or another browser-compatible database.

Design:

Local repository
Sync queue
Conflict handling
Server repository

Document:

ONLINE
OFFLINE
SYNCING
SYNC FAILED

states.

============================================================
52. CONFLICT RESOLUTION
============================================================

Prevent duplicate habit completions.

Use:

Idempotency
Stable record IDs
Updated timestamps
Mutation identifiers

Define conflict-resolution behavior explicitly.

============================================================
53. SECURITY
============================================================

Implement:

Authentication
Authorization
Ownership checks
Input validation
Rate limiting
Security headers
Secure cookies
CORS policy
CSRF protection where applicable
SQL injection protection
XSS mitigation
Secret management
Secure OAuth
Password hashing

Every user-owned resource must verify ownership server-side.

Never trust user_id supplied by the browser as authorization.

============================================================
54. PRIVACY
============================================================

Provide architecture for:

Download My Data

Delete My Data

Delete Account

Privacy Policy

Terms

Do not collect unnecessary data.

============================================================
55. EXPORT
============================================================

Allow export where practical:

CSV
JSON
PDF progress report

Architect future spreadsheet import/export support.

============================================================
56. RESPONSIVE DESIGN
============================================================

Test:

320px
360px
390px
430px
768px
1024px
1280px
1440px
1920px

No horizontal overflow on normal mobile pages.

Charts must resize correctly.

============================================================
57. LOADING EXPERIENCE
============================================================

Use:

Skeleton loaders
Progress indicators
Suspense boundaries
Optimistic UI

Avoid unnecessary full-screen spinners.

============================================================
58. EMPTY STATES
============================================================

Create attractive empty states.

Examples:

NO HABITS YET

Create your first habit and start building momentum.

[ + CREATE HABIT ]

NO GOALS YET

Turn your next ambition into a measurable goal.

[ + CREATE GOAL ]

============================================================
59. ERROR EXPERIENCE
============================================================

Never expose raw stack traces.

Provide human-readable messages.

Include:

404
403
500
Offline
Network failure
Authentication expired

Create polished error pages.

============================================================
60. MONITORING
============================================================

Use OpenTelemetry.

Instrument important:

HTTP requests
NestJS services
Database calls
External dependencies
Background processes

Use trace IDs where appropriate.

============================================================
61. PROMETHEUS
============================================================

Expose production-safe metrics.

Track:

Request count
Latency
Error rate
Database performance
Cache performance
Authentication failures
API availability

Avoid exposing sensitive data as metric labels.

============================================================
62. GRAFANA
============================================================

Provide Grafana configuration/dashboard guidance for:

API Health

Request Rate

P95/P99 Latency

Error Rate

PostgreSQL

Redis

Authentication

Application Health

============================================================
63. HEALTH ENDPOINTS
============================================================

Create:

/health

/health/live

/health/ready

Readiness should verify critical dependencies appropriately.

============================================================
64. DOCKER
============================================================

Containerize:

Next.js Web

NestJS API

PostgreSQL

Redis

Prometheus

Grafana

Provide a development docker-compose setup.

Use health checks.

Use persistent volumes where required.

============================================================
65. CI/CD
============================================================

Create GitHub Actions.

On Pull Request:

Install
Lint
Typecheck
Unit Tests
Integration Tests
Build

On approved production branch:

Build production artifacts
Build Docker images
Run security checks
Deploy according to documented environment

Use dependency caching.

Never expose secrets in logs.

============================================================
66. TESTING
============================================================

Use appropriate tools such as:

Vitest/Jest
React Testing Library
Supertest
Playwright

UNIT TEST:

Streak calculations
Completion percentages
Scheduling
Goal progress
Analytics

INTEGRATION TEST:

Authentication
Habit CRUD
Habit completion
Goals
Milestones
Reviews

E2E TEST:

Register
Login
Complete onboarding
Create habit
Complete habit
View streak
Create goal
Complete milestone
View analytics
Switch theme
Logout

============================================================
67. README
============================================================

Create an excellent README containing:

Product overview

Architecture

Technology stack

Repository structure

Prerequisites

Installation

Environment variables

PostgreSQL setup

Prisma setup

Redis setup

Docker setup

Local development

Testing

OpenAPI documentation

Monitoring

Production build

Deployment

PWA behavior

Offline architecture

Troubleshooting

============================================================
68. ENVIRONMENT CONFIGURATION
============================================================

Create:

.env.example

Include placeholders only.

Never include actual secrets.

============================================================
69. SEED DATA
============================================================

Create realistic development/demo data.

Example habits:

Drink 3L Water
Workout
Read 30 Minutes
Learn a Language
Meditate
Sleep Before 11 PM
Avoid Doomscrolling

Example goals:

Complete Online Course
Workout 20 Days
Read 12 Books
Build Morning Routine

============================================================
70. SEO — PUBLIC LANDING PAGE
============================================================

Implement:

Metadata
Open Graph
Twitter metadata
Sitemap
robots.txt
Canonical URLs
Structured data where appropriate

Authenticated private pages should not be indexed.

============================================================
71. PRODUCTION QUALITY
============================================================

Before completion verify:

✓ Frontend builds
✓ Backend builds
✓ Database migrations work
✓ Prisma client works
✓ Redis integration works
✓ Authentication works
✓ Google login works
✓ Registration works
✓ Landing page works
✓ 3D experience works
✓ Mobile layout works
✓ Desktop layout works
✓ Habit CRUD works
✓ Habit completion works
✓ Streak engine works
✓ Goals work
✓ Milestones work
✓ Routines work
✓ Focus timer works
✓ Reviews work
✓ Analytics work
✓ Heatmap works
✓ Light mode works
✓ Dark mode works
✓ PWA works
✓ Offline strategy works
✓ OpenAPI works
✓ Docker works
✓ CI works
✓ Tests pass
✓ Health checks work
✓ Monitoring works

============================================================
72. CRITICAL DEVELOPMENT RULE
============================================================

DO NOT build the entire project as fake UI first.

Build vertically working functionality.

Recommended implementation order:

PHASE 1
Architecture + monorepo

PHASE 2
PostgreSQL + Prisma

PHASE 3
NestJS API foundation

PHASE 4
Authentication

PHASE 5
Next.js application shell

PHASE 6
Landing page + login

PHASE 7
Habit CRUD

PHASE 8
Habit completion + scheduling

PHASE 9
Streak engine

PHASE 10
Dashboard

PHASE 11
Goals + milestones

PHASE 12
Routines

PHASE 13
Focus

PHASE 14
Analytics + heatmap

PHASE 15
PWA/offline synchronization

PHASE 16
Redis

PHASE 17
Monitoring

PHASE 18
Docker

PHASE 19
Testing

PHASE 20
CI/CD + production hardening

At the end of each phase:

RUN THE APPLICATION.

RUN RELEVANT TESTS.

FIX ERRORS BEFORE CONTINUING.

Do not knowingly leave broken code for a later phase.

============================================================
73. NO PLACEHOLDER IMPLEMENTATION
============================================================

Do not create buttons that do nothing.

Do not create charts with fake static values once real data exists.

Do not create fake authentication.

Do not create fake API responses.

Do not leave TODO comments for essential functionality.

Do not create pages that visually exist but have no backend functionality.

Every major user-facing feature must connect through:

UI
↓
Validation
↓
REST API
↓
NestJS service
↓
Prisma
↓
PostgreSQL
↓
Response
↓
TanStack Query
↓
Updated UI

============================================================
74. FINAL EXPECTATION
============================================================

The goal is not merely to create "a habit tracker."

Create a flagship productivity platform with:

🔥 Premium 3D experience
🪟 Glassmorphism UI
🌙 Light/Dark themes
🔐 Authentication
📱 Mobile-first experience
💻 Desktop dashboard
✅ Habit tracking
📅 Scheduling
🔥 Streaks
🎯 Goals
🪜 Milestones
🌅 Routines
⏱ Focus tracking
📊 Advanced analytics
🟩 Heatmaps
🏆 Achievements
🧠 Smart insights
🔔 Reminders
📲 PWA
📴 Offline capability
⚡ Redis
🐘 PostgreSQL
🔷 Prisma
🟢 NestJS
⚛ React
▲ Next.js
🐳 Docker
🔄 GitHub Actions
📡 OpenTelemetry
📈 Prometheus
📊 Grafana

The finished application must be:

FAST
SECURE
SCALABLE
RESPONSIVE
ACCESSIBLE
VISUALLY EXTRAORDINARY
MAINTAINABLE
TESTED
PRODUCTION-READY

It should look and feel like a premium commercial product built by an experienced product design and engineering team.

============================================================
FINAL COMMAND
============================================================

START FROM AN EMPTY PROJECT AND BUILD THE APPLICATION.

Do not stop after planning the architecture.

Do not give me only code snippets.

Do not give me only a tutorial.

Do not give me only UI mockups.

Do not build only the landing page.

Do not build only authentication.

Do not build only the dashboard.

CREATE THE COMPLETE WORKING CODEBASE.

Start by establishing the monorepo and architecture, then implement the application phase by phase.

After every major phase:

1. Run type checking.
2. Run linting.
3. Run relevant tests.
4. Run/build the application.
5. Fix errors.
6. Continue only when the current phase works.

Prioritize correctness, security, responsiveness, accessibility, performance, maintainability, and visual quality.

The final result should be one of the highest-quality Habit & Goal Tracking applications possible with this technology stack.
