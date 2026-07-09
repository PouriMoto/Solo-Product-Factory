# DECISION-LOGIC.md
Status: Draft
Purpose:
این فایل صندوق ایده‌های در انتظار است — هر ایده‌ی تازه (از تجربه، مقاله، یا اشتباه یک پروژه) اول اینجا نوشته می‌شود، نه مستقیم در فایل اصلی.

## قبل از اضافه‌کردن ایده‌ی تازه، اینجا را چک کن (آیا قبلاً پوشش داده شده؟)
STD: 01-CONSTITUTION / 02-PHASES / 03-REUSE-FIRST / 04-ANTIPATTERNS / 05-CHECKLIST / 06-PROMPTS / 08-PROJECT-STATE
SPF: 01-CONSTITUTION / 02-BLUEPRINT-TEMPLATE / 03-EVIDENCE-GATES / 04-KPI-FRAMEWORK / 05-B2B-DATA-MODEL / 06-PORTFOLIO-RULES / 07-LEARNING-LOG-TEMPLATE

اگر پوشش داده نشده، این فرمت را زیر همین جمع‌بندی اضافه کن:

## [عنوان ایده کوتاه]
Priority: Low / Medium / High
Status: 🆕 New
از کجا اومد: [کدوم پروژه/تجربه]
مشکل: [یک-دو جمله]
پیشنهاد: [یک-دو جمله]

قانون ورود به استاندارد اصلی: فقط وقتی یک ایده در ۲-۳ پروژه‌ی متوالی واقعاً لازم شد (نه فقط یک‌بار)، وارد فایل اصلی STD/SPF می‌شود.

==================================================
1. THINK BEFORE BUILD
Priority: High
==================================================

مشکل:

اکثر مدل‌های AI به محض دریافت درخواست شروع به طراحی Solution و تولید کد می‌کنند.

در حالی که هنوز:

- مسئله دقیق مشخص نشده
- محدودیت‌ها مشخص نیست
- Success Criteria مشخص نیست
- فرضیات بررسی نشده

تصمیم:

قبل از هر Feature ابتدا Problem Analysis انجام شود.

AI نباید قبل از درک مسئله وارد مرحله طراحی شود.

ممکن است فایل جدیدی مانند:

00-PROBLEM-FIRST.md

ایجاد شود.

موضوعات احتمالی:

- Problem Statement
- Users
- Constraints
- Assumptions
- Non Goals
- Success Criteria
- Risks

--------------------------------------------------

==================================================
2. FOUNDATION FIRST
Priority: Very High
==================================================

در حال حاضر Reuse First وجود دارد.

اما کافی نیست.

قبل از Build باید بررسی شود:

Authentication

Authorization

Storage

Database

Queue

Notification

Analytics

Logging

Monitoring

Billing

OCR

Maps

Search

Email

SMS

Image Processing

AI Provider

Workflow Engine

Scheduler

Object Storage

Realtime

و سایر Foundation ها

هدف:

قبل از نوشتن کد
بررسی شود آیا Foundation مناسب وجود دارد یا خیر.

--------------------------------------------------

==================================================
3. ARCHITECTURE DECISION RECORD (ADR)
Priority: High
==================================================

یکی از کمبودهای فعلی:

هیچ جا ثبت نمی‌شود که

چرا

یک تصمیم معماری گرفته شده است.

مثلاً

چرا Prisma؟

چرا Supabase؟

چرا TanStack Query؟

چرا NextJS؟

چرا Repository Pattern؟

بعد از چند ماه کسی دلیل تصمیم را نمی‌داند.

ایده:

پوشه

adr/

یا

DECISIONS/

ایجاد شود.

هر تصمیم مهم ثبت شود.

--------------------------------------------------

==================================================
4. ENTITY CATALOG
Priority: High
==================================================

پیشنهاد:

برای هر پروژه

Entity ها

در یک فایل ثبت شوند.

مثلاً

Customer

Order

Invoice

Vehicle

Game

Card

و ...

برای هر Entity

Fields

Validation

Repository

Permission

Lifecycle

Owner

Relations

ثبت گردد.

--------------------------------------------------

==================================================
5. DATA FLOW DOCUMENT
Priority: High
==================================================

در حال حاضر

Data Flow

داخل Prompt وجود دارد.

پیشنهاد:

فایل مستقل داشته باشد.

برای هر Entity

Flow

ثبت شود.

مثلاً

Customer

↓

Repository

↓

Database

↓

Analytics

↓

Dashboard

--------------------------------------------------

==================================================
6. ACCEPTANCE CRITERIA
Priority: Medium
==================================================

قبل از اینکه AI اعلام کند

Feature Complete

باید بررسی کند:

Loading

Error State

Permission

Responsive

Accessibility

Empty State

Performance

Security

Logging

Analytics

همگی بررسی شده‌اند یا خیر.

--------------------------------------------------

==================================================
7. MIGRATION GUIDE
Priority: High
==================================================

اکثر پروژه‌ها مسیر زیر را دارند.

POC

↓

LocalStorage

↓

Database

↓

Production

↓

Scale

بنابراین

راهنمای Migration

باید فایل مستقل داشته باشد.

--------------------------------------------------

==================================================
8. PRODUCT THINKING
Priority: High
==================================================

استاندارد فعلی بیشتر روی Code تمرکز دارد.

در حالی که

Product Thinking

کمتر پوشش داده شده.

قبل از Feature

این سوال‌ها باید پاسخ داده شوند:

چرا این Feature؟

برای چه کسی؟

چه مشکلی را حل می‌کند؟

اگر حذف شود چه می‌شود؟

آیا واقعاً لازم است؟

--------------------------------------------------

==================================================
9. BUILD vs BUY SCORE
Priority: High
==================================================

الان فقط قانون Reuse وجود دارد.

اما بهتر است

یک Decision Matrix وجود داشته باشد.

مثلاً

هزینه ساخت

هزینه نگهداری

ریسک امنیت

مزیت رقابتی

Vendor Lock-in

زمان توسعه

Community

Documentation

و ...

بر اساس امتیاز

تصمیم گرفته شود.

--------------------------------------------------

==================================================
10. PROJECT FOUNDATION MAP
Priority: Medium
==================================================

در ابتدای پروژه

AI

باید لیست کند:

چه Foundation هایی استفاده خواهند شد.

مثلاً

Auth

Supabase Auth

Storage

Supabase Storage

Analytics

PostHog

Logging

Sentry

Database

Postgres

Deployment

Vercel

Monitoring

Better Stack

و ...

تا بعداً

Foundation جدید ساخته نشود.

--------------------------------------------------

==================================================
11. FEATURE COMPLETENESS
Priority: Medium
==================================================

AI نباید فقط بگوید

Done

بلکه مشخص کند:

Functional Complete

Architecture Complete

Test Ready

Production Ready

Documentation Ready

هر کدام جداگانه.

--------------------------------------------------

==================================================
12. DECISION BEFORE CODING
Priority: High
==================================================

قبل از هر Feature

AI ابتدا تصمیم‌ها را اعلام کند.

مثلاً

Data Source

Repository

Caching

Permission

Validation

Storage

External Services

Dependency

سپس وارد کدنویسی شود.

--------------------------------------------------

==================================================
13. PROJECT KNOWLEDGE BASE
Priority: Medium
==================================================

در طول پروژه

دانش تولید می‌شود.

مثلاً

Architecture

Entities

Flows

ADR

Lessons Learned

Known Issues

Patterns

این دانش نباید داخل Chat گم شود.

--------------------------------------------------

==================================================
14. LESSONS LEARNED
Priority: Medium
==================================================

بعد از هر Sprint

اشتباهات مهم

ثبت شوند.

هدف:

AI

در پروژه‌های بعد

همان اشتباه را تکرار نکند.

--------------------------------------------------

==================================================
15. STANDARD EVOLUTION
Priority: High
==================================================

این استاندارد

نباید ثابت بماند.

قانون:

بعد از هر 3 تا 5 پروژه

بازبینی شود.

اگر قانونی

بیش از حد سخت

یا

غیرعملی

بود

اصلاح شود.

اگر خطای جدیدی

چند بار تکرار شد

به Constitution

Checklist

یا Antipatterns

اضافه شود.

==================================================
جمع‌بندی
==================================================

در بازبینی انجام‌شده مشخص شد که نسخه فعلی استاندارد تقریباً بخش Code Quality و بخش زیادی از Architecture را پوشش می‌دهد.

نسخه‌های بعدی بهتر است سه لایه مستقل داشته باشند:

Layer 1
Thinking
(Problem First + Product Thinking + Build vs Buy)

Layer 2
Architecture
(Foundation + ADR + Entity + Data Flow + Migration)

Layer 3
Execution
(Constitution + Reuse + Antipatterns + Checklist + Prompts)

این ساختار احتمالاً استاندارد را از یک "راهنمای کدنویسی" به یک "سیستم تصمیم‌گیری برای توسعه محصول با AI" تبدیل خواهد کرد.
