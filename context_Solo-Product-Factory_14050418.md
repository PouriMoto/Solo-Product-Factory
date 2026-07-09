# PROJECT SUMMARY

Project: Solo-Product-Factory-main
Generated: 2026-07-09T18:52:23
Total files: 19
Approx Tokens: 15078

Languages:
- Markdown

---

# DIRECTORY TREE

├── DECISION-LOGIC.md
├── README.fa.md
├── README.md
    ├── 01-CONSTITUTION.md
    ├── 02-BLUEPRINT-TEMPLATE.md
    ├── 03-EVIDENCE-GATES.md
    ├── 04-KPI-FRAMEWORK.md
    ├── 05-B2B-DATA-MODEL.md
    ├── 06-PORTFOLIO-RULES.md
    ├── 07-LEARNING-LOG-TEMPLATE.md
    ├── 08-PROJECT-STATE.md
    ├── README.md
    ├── 01-CONSTITUTION.md
    ├── 02-PHASES.md
    ├── 03-REUSE-FIRST.md
    ├── 04-ANTIPATTERNS.md
    ├── 05-CHECKLIST.md
    ├── 06-PROMPTS.md
    ├── README.md

---

# FILE INDEX

001. DECISION-LOGIC.md
002. README.fa.md
003. README.md
004. SPF/01-CONSTITUTION.md
005. SPF/02-BLUEPRINT-TEMPLATE.md
006. SPF/03-EVIDENCE-GATES.md
007. SPF/04-KPI-FRAMEWORK.md
008. SPF/05-B2B-DATA-MODEL.md
009. SPF/06-PORTFOLIO-RULES.md
010. SPF/07-LEARNING-LOG-TEMPLATE.md
011. SPF/08-PROJECT-STATE.md
012. SPF/README.md
013. VibeCoding-STD/01-CONSTITUTION.md
014. VibeCoding-STD/02-PHASES.md
015. VibeCoding-STD/03-REUSE-FIRST.md
016. VibeCoding-STD/04-ANTIPATTERNS.md
017. VibeCoding-STD/05-CHECKLIST.md
018. VibeCoding-STD/06-PROMPTS.md
019. VibeCoding-STD/README.md

---

# FILES

---

<FILE path="DECISION-LOGIC.md" tokens="1970" lines="609">

```md
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

```

</FILE>

---

<FILE path="README.fa.md" tokens="1560" lines="524">

```md
Folder:
Solo-Product-Factory/

File:
README.fa.md

# Solo Product Factory (SPF)

نسخه: 1.0

---

# Solo Product Factory چیست؟

**Solo Product Factory (SPF)** یک سیستم کاری (Operating System) برای یک **Solo Entrepreneur** است که با کمک هوش مصنوعی و Vibe Coding، محصولات B2B، SaaS و AI را به‌صورت سریع، تکرارپذیر و قابل توسعه تولید می‌کند.

هدف SPF ساخت «نرم‌افزار کامل» نیست.

هدف SPF ساخت سریع محصولاتی است که با مشتری واقعی اعتبارسنجی شوند و در نهایت به یک کسب‌وکار واقعی تبدیل شوند.

SPF یک Framework نیست.

SPF یک زبان برنامه‌نویسی نیست.

SPF یک استاندارد کدنویسی هم نیست.

SPF یک سیستم تصمیم‌گیری، ساخت محصول و یادگیری است.

---

# مأموریت (Mission)

تبدیل این مسیر:

ایده

↓

کدنویسی

↓

امید داشتن به موفقیت

به این مسیر:

ایده

↓

Discovery

↓

Evidence

↓

Blueprint

↓

MVP

↓

Evidence

↓

Stabilize & Optimize

↓

Evidence

↓

Scale

در پایان هر مرحله فقط یک سؤال وجود دارد:

**آیا شواهد کافی برای ورود به مرحله بعد وجود دارد؟**

اگر پاسخ خیر باشد،

باید به مرحله قبل بازگردیم.

---

# فلسفه اصلی

یادگیری از کدنویسی مهم‌تر است.

اعتبارسنجی از معماری مهم‌تر است.

رفتار مشتری از نظر مشتری مهم‌تر است.

سرعت از کامل بودن مهم‌تر است.

حل یک مشکل واقعی از ساخت ده قابلیت مهم‌تر است.

---

# مهم‌ترین KPI

مهم‌ترین KPI این سیستم:

تبدیل

ایده

↓

اولین مشتری پرداخت‌کننده

در کمترین زمان ممکن است.

تمام تصمیم‌های فنی، محصولی و تجاری باید این KPI را بهبود دهند.

---

# فلسفه محصول

هر محصول فقط **یک مشکل اصلی** را حل می‌کند.

هر محصول فقط **یک KPI اصلی** دارد.

هر Feature فقط **یک فرضیه** را آزمایش می‌کند.

اگر حذف یک Feature باعث نشود مشتری ثبت‌نام نکند یا پول ندهد،

آن Feature هنوز لازم نیست.

اگر توضیح محصول بیشتر از ۳۰ ثانیه طول بکشد،

محصول بیش از حد پیچیده است.

اگر ساخت MVP بیشتر از حدود دو روز زمان ببرد،

دامنه محصول بیش از حد بزرگ است و باید کوچک‌تر شود.

---

# چرخه استاندارد توسعه محصول

## فاز صفر

Discovery

خروجی:

Blueprint

↓

Evidence

↓

## فاز اول

MVP

هدف:

اعتبارسنجی اولین فرضیه

↓

Evidence

↓

## فاز دوم

Stabilize & Optimize

هدف:

تبدیل MVP به محصول پایدار

↓

Evidence

↓

## فاز سوم

Scale

هدف:

رشد محصول

---

# چهار ستون اصلی SPF

## ۱. Blueprint

Blueprint مشخص می‌کند:

- چه چیزی ساخته شود.
- برای چه کسی ساخته شود.
- چه مشکلی را حل می‌کند.
- مدل درآمد چیست.
- KPI چیست.
- MVP شامل چه بخش‌هایی است.
- چه چیزهایی عمداً ساخته نمی‌شوند.

Blueprint همیشه قبل از اولین خط کد تولید می‌شود.

---

## ۲. Foundation Library

Foundation کتابخانه دانش و تصمیم‌های قابل استفاده مجدد است.

نمونه‌ها:

- احراز هویت
- مجوزها
- RBAC
- Billing
- پرداخت
- پایگاه داده
- ذخیره‌سازی
- اعلان‌ها
- Analytics
- AI
- استقرار
- مانیتورینگ
- تست
- Cache
- Multi-Tenant
- API
- Integration

هر تصمیم فقط یک بار گرفته می‌شود.

سپس در تمام پروژه‌ها استفاده می‌شود.

اول **Reuse**

بعد **Build**

---

## ۳. VibeCoding-STD

استاندارد توسعه فنی داخل SPF تعریف نمی‌شود.

تمام قوانین توسعه در Repository مستقل

**VibeCoding-STD**

قرار دارند.

این استاندارد شامل موارد زیر است:

- قوانین کدنویسی
- معماری نرم‌افزار
- Workflow توسعه
- Promptها
- Templateها
- Checklistها
- Anti-patternها

SPF مشخص می‌کند:

**چه چیزی ساخته شود.**

VibeCoding-STD مشخص می‌کند:

**چگونه ساخته شود.**

---

## ۴. Learning System

هر محصول باید باعث بهتر شدن محصول بعدی شود.

بعد از هر پروژه باید پاسخ داده شود:

چه چیزی درست بود؟

چه چیزی اشتباه بود؟

کدام فرضیه رد شد؟

کدام Prompt بهتر شد؟

چه چیزی باید وارد Foundation شود؟

چه چیزی باید حذف شود؟

دانش از پروژه‌ها استخراج می‌شود.

و این دانش سرعت پروژه‌های بعدی را افزایش می‌دهد.

---

# سیستم Evidence

هیچ مرحله‌ای بدون Evidence تمام نمی‌شود.

نمونه‌های Evidence:

- مصاحبه با مشتری
- لیست انتظار
- پیش‌ثبت‌نام
- ثبت‌نام
- استفاده واقعی
- بازگشت کاربر
- پرداخت
- معرفی مشتری
- داده‌های Analytics
- درخواست‌های پشتیبانی

Evidence همیشه از حدس مهم‌تر است.

---

# فلسفه کسب‌وکار

محصولات عمدتاً B2B هستند.

پرداخت‌کننده معمولاً کسب‌وکار است.

کاربر نهایی فقط از محصول استفاده می‌کند.

اکثر محصولات به‌صورت Multi-Tenant طراحی می‌شوند.

هدف ساخت پلتفرم‌های قابل رشد است، نه پروژه‌های تک‌منظوره.

---

# فلسفه توسعه

کوچک فکر کن.

کوچک بساز.

سریع منتشر کن.

دائماً اندازه‌گیری کن.

سریع یاد بگیر.

مرتب بهبود بده.

قبل از اعتبارسنجی بهینه‌سازی نکن.

قبل از اعتبارسنجی معماری پیچیده نساز.

Feature غیرضروری اضافه نکن.

---

# چارچوب تصمیم‌گیری

قبل از هر تصمیم این سؤال‌ها را بپرس:

آیا این کار زمان رسیدن به اولین مشتری پرداخت‌کننده را کاهش می‌دهد؟

آیا این Feature یک فرضیه را آزمایش می‌کند؟

آیا پیچیدگی غیرضروری ایجاد می‌کند؟

آیا بعداً دوباره قابل استفاده است؟

آیا باید وارد Foundation شود؟

اگر پاسخ اکثر سؤال‌ها «خیر» باشد،

آن را نساز.

---

# مدیریت چند محصول

هم‌زمان چند MVP ساخته نمی‌شود.

ابتدا چرخه یادگیری محصول فعلی کامل می‌شود.

محصول بعدی فقط زمانی شروع می‌شود که محصول قبلی:

به KPI هدف رسیده باشد

یا

آگاهانه متوقف شده باشد.

---

# ساختار Repository

### SPF-001

معرفی Solo Product Factory

---

### SPF-002

چرخه عمر محصول

---

### SPF-003

Foundation و سیستم دانش

---

### SPF-004

Blueprint System

استاندارد طراحی محصول قبل از شروع توسعه

---

### SPF-005

Evidence System

قوانین اعتبارسنجی و تصمیم Go / No-Go

---

### SPF-006

Business Operating System

مدل کسب‌وکار، قیمت‌گذاری، B2B، Multi-Tenant

---

### SPF-007

Product Portfolio

مدیریت چند محصول و تصمیم‌گیری برای ساخت محصول بعدی

---

### SPF-008

Learning System

ثبت تجربه‌ها و تبدیل آن‌ها به دانش قابل استفاده مجدد

---

### SPF-009

Decision Framework

چارچوب تصمیم‌گیری‌های فنی، محصولی و تجاری

---

### SPF-010

Product Metrics

KPIها، North Star Metric، Retention، Activation، Revenue، Conversion و سایر معیارهای کلیدی

---

# Reference

پوشه Reference شامل منابع خارجی و دانش قابل استفاده مجدد است.

نمونه‌ها:

- VibeCoding-STD
- Tech Stack
- Foundation Modules
- Prompt Library
- Tools
- Templateها

---

# Constitution

Constitution قوانین تغییرناپذیر سیستم را تعریف می‌کند.

مانند:

- دو روزه MVP بساز.
- هر محصول فقط یک مشکل.
- هر محصول فقط یک KPI.
- هر Feature فقط یک فرضیه.
- رفتار مشتری مهم‌تر از حرف مشتری است.
- اول Evidence، بعد توسعه.
- اول Reuse، بعد Build.
- اول Validation، بعد Optimization.
- اول Optimization، بعد Scale.

اگر هر سند دیگری با Constitution تضاد داشته باشد،

همیشه Constitution ملاک تصمیم است.

---

# جمله پایانی

بساز.

اندازه‌گیری کن.

یاد بگیر.

تکرار کن.

موفقیت نتیجه ساخت نرم‌افزار نیست.

موفقیت نتیجه ساخت یک چرخه تکرارپذیر برای خلق کسب‌وکارهای موفق است.

```

</FILE>

---

<FILE path="README.md" tokens="1527" lines="547">

```md
Folder:
Solo-Product-Factory/

File:
README.md

# Solo Product Factory (SPF)

Version: 1.0

---

# What is Solo Product Factory?

Solo Product Factory (SPF) is a practical operating system for a Solo Entrepreneur who builds B2B SaaS and AI products using AI-assisted (Vibe Coding) development.

The objective is NOT to build perfect software.

The objective is to repeatedly transform ideas into validated businesses as quickly and cheaply as possible.

SPF is not a framework.

SPF is not a coding standard.

SPF is a decision-making and product-building system.

---

# Mission

Transform this:

Idea

↓

Coding

↓

Hope

Into this:

Idea

↓

Discovery

↓

Evidence

↓

Blueprint

↓

MVP

↓

Evidence

↓

Optimize

↓

Evidence

↓

Scale

Every phase must produce evidence before moving to the next.

---

# Core Philosophy

Learning is more valuable than software.

Evidence is more valuable than opinions.

Customer behavior is more valuable than customer feedback.

Speed is more valuable than perfection.

Validation is more valuable than architecture.

One solved problem is more valuable than ten unfinished ideas.

---

# Main KPI

The primary KPI of SPF is NOT:

- Features
- Architecture
- Code Quality
- Clean Code
- GitHub Stars

The primary KPI is:

Idea

↓

First Paying Customer

as quickly as possible.

Every decision must improve this KPI.

---

# Product Philosophy

Every product solves ONE core problem.

Every product has ONE North Star KPI.

Every feature validates ONE hypothesis.

If removing a feature does not reduce customer adoption,

the feature should not exist.

If explaining the product takes more than 30 seconds,

the product is too complicated.

If building the MVP takes more than two days,

the MVP is too large.

Reduce scope.

Never reduce learning.

---

# Product Lifecycle

Phase 0

Discovery

Output:

Blueprint

↓

Evidence

↓

Phase 1

MVP

Validate one hypothesis.

↓

Evidence

↓

Phase 2

Stabilize & Optimize

Build a reliable product.

↓

Evidence

↓

Phase 3

Scale

Grow only after validation.

---

# Four Core Systems

## 1. Blueprint

Blueprint defines:

- Problem
- Customer
- Value Proposition
- Business Model
- Success Metrics
- MVP Scope
- Architecture
- What NOT to build

Blueprint exists before code.

---

## 2. Foundation Library

Foundation stores reusable knowledge.

Examples:

Authentication

Authorization

RBAC

Billing

Payments

Database

Storage

Analytics

Notifications

AI

Deployment

Monitoring

Testing

Caching

Multi-Tenancy

API

Integrations

Every decision should be made once and reused forever.

Reuse before Build.

---

## 3. VibeCoding-STD

Technical implementation is NOT defined here.

Technical standards are managed in the independent repository:

VibeCoding-STD

It contains:

Coding Rules

Architecture Rules

Prompt Standards

Development Workflow

Templates

Checklists

Anti-patterns

SPF decides WHAT should be built.

VibeCoding-STD defines HOW it is built.

---

## 4. Learning System

Every finished product improves the next one.

After every project ask:

What worked?

What failed?

Which assumptions were wrong?

Which prompts improved?

Which decisions belong in Foundation?

Which decisions should be removed?

Products build knowledge.

Knowledge builds better products.

---

# Evidence System

No phase finishes without evidence.

Evidence includes:

Customer Interviews

Pre-orders

Waiting List

Registrations

Usage

Retention

Payments

Referrals

Analytics

Support Requests

Evidence always wins over assumptions.

---

# Business Philosophy

Primary products are B2B.

Businesses pay.

Customers use.

Most products are Multi-Tenant.

The goal is to create reusable business platforms rather than isolated applications.

---

# Development Philosophy

Think small.

Build small.

Release early.

Measure continuously.

Learn quickly.

Improve continuously.

Avoid premature optimization.

Avoid premature architecture.

Avoid unnecessary features.

---

# Decision Framework

Before making any decision ask:

Does this reduce time to the first paying customer?

Does this validate a business hypothesis?

Does this reduce unnecessary complexity?

Can it be reused?

Does it belong in Foundation?

If the answer is mostly "No",

do not build it.

---

# Product Portfolio Rules

Never build many MVPs simultaneously.

Complete the learning cycle first.

A new product starts only when the previous product has:

Reached its KPI

or

Been intentionally discontinued.

---

# Repository Structure

SPF-001

Solo Product Factory Overview

SPF-002

Product Lifecycle

SPF-003

Foundation & Knowledge System

SPF-004

Blueprint System

How every product is designed before coding.

SPF-005

Evidence System

Validation rules and Go / No-Go decisions.

SPF-006

Business Operating System

Business model, pricing, B2B strategy, Multi-Tenant thinking.

SPF-007

Product Portfolio

Managing multiple products and deciding what to build next.

SPF-008

Learning System

Capturing lessons learned and evolving Foundation.

SPF-009

Decision Framework

Build vs Buy, Pivot, Kill, Scale, Technical and Business decisions.

SPF-010

Product Metrics

North Star KPI, Activation, Retention, Revenue, Conversion and growth metrics.

---

# References

Reference documents contain external knowledge and reusable resources.

Examples:

VibeCoding-STD

Recommended Tech Stack

Foundation Modules

Tools

Templates

Prompt Library

---

# Constitution

The Constitution defines immutable rules.

Examples:

Build in two days.

One Product = One Problem.

One Product = One KPI.

One Feature = One Hypothesis.

Customer behavior beats customer opinion.

Evidence before assumptions.

Reuse before Build.

Validation before Optimization.

Optimization before Scale.

If these rules conflict with any other document,

the Constitution always wins.

---

# Final Principles

Build.

Measure.

Learn.

Repeat.

Small wins beat perfect plans.

Evidence beats assumptions.

Products create knowledge.

Knowledge creates better products.

The goal is not writing software.

The goal is building repeatable businesses.

```

</FILE>

---

<FILE path="SPF/01-CONSTITUTION.md" tokens="913" lines="71">

```md
# 01 — Constitution

قوانین این فایل در تمام محصولات و تمام فازها بدون استثنا اعمال می‌شوند.
اگر جایی نقض یکی از این قوانین لازم به نظر رسید، آن نقض باید آگاهانه و مکتوب باشد، نه ناخواسته.

این فایل باید همیشه در دسترس باشد — قبل از شروع Blueprint هر محصول تازه، این را مرور کن.

---

## قانون ۱ — Evidence قبل از توسعه بیشتر

هیچ فازی بدون Evidence واقعی (نه حدس، نه «به‌نظرم خوب میاد») تمام نمی‌شود.
اگر در پایان یک فاز Evidence کافی نبود، دو راه داری: برگرد و محصول را کوچک‌تر کن، یا برو سراغ Evidence جمع کردن — نه اینکه Feature تازه اضافه کنی.

**تشخیص نقض:** اگر داری کد می‌نویسی ولی جواب این سؤال «آخرین باری که یک نفر غیر از خودم از این استفاده کرد کی بود؟» بیش از یک هفته قبل است، این قانون نقض شده.

## قانون ۲ — هر محصول یک مشکل، یک KPI

هر محصول فقط یک مشکل اصلی را حل می‌کند و فقط یک KPI اصلی دارد.
اگر محصول دو مشکل مجزا را حل می‌کند، احتمالاً دو محصول است — طبق `04-KPI-FRAMEWORK.md` جدا کن.

**تشخیص نقض:** اگر توضیح محصول به یک نفر بیشتر از ۳۰ ثانیه طول می‌کشد، یا مجبوری از "و" برای وصل کردن دو قابلیت اصلی استفاده کنی، این قانون نقض شده.

## قانون ۳ — محدودیت زمانی MVP

ساخت اولین نسخه‌ی قابل تست (نه نسخه‌ی کامل) نباید بیشتر از ۲ روز طول بکشد.
اگر بیشتر طول کشید، دامنه محصول بزرگ است — چیزی را حذف کن، نه اینکه زمان را افزایش بده.

«۲ روز» یعنی باریک‌ترین ورژنی که می‌شود جلوی یک نفر واقعی گذاشت و واکنش گرفت — نه محصول کامل با همه‌ی Feature‌ها. جزئیات دقیق در `02-BLUEPRINT-TEMPLATE.md` بخش «چه چیزی عمداً ساخته نمی‌شود».

## قانون ۴ — یک هفته برای اولین مشتری

بعد از ساخت MVP، حداکثر یک هفته وقت داری تا آن را جلوی مشتری واقعی (نه دوست، نه آشنا، نه خودت) ببری.
اگر در این یک هفته حداقل یک مشتری واقعی (طبق تعریف در `03-EVIDENCE-GATES.md`) به‌دست نیامد، محصول را کوچک‌تر کن یا فرضیه را عوض کن.

**تشخیص نقض:** اگر یک هفته از تمام‌شدن MVP گذشته و هنوز کسی خارج از دایره‌ی نزدیکانت آن را ندیده، این قانون نقض شده — این خودش مهم‌ترین علامت هشدار در پروژه‌های قبلی بود.

## قانون ۵ — رفتار مهم‌تر از حرف

آنچه مشتری واقعاً انجام می‌دهد (کلیک می‌کند، پول می‌دهد، برمی‌گردد) معتبرتر از آنچه می‌گوید («ایده‌ی خوبیه»، «حتماً استفاده می‌کنم») است.
تصمیم‌های Go/No-Go را بر اساس رفتار بگیر، نه بر اساس تعریف و تمجید کلامی.

## قانون ۶ — Reuse قبل از Build

قبل از ساخت هر زیرساخت (Auth، دیتابیس، پرداخت، Analytics)، بررسی کن آیا نسخه‌ی آماده وجود دارد.
جزئیات فنی این قانون در Repository جدا `VibeCoding-STD` است؛ اینجا فقط اصل تصمیم‌گیری اهمیت دارد: وقت را صرف مشکل اصلی محصول کن، نه بازسازی چیزی که همه دارند.

## قانون ۷ — Payer ≠ End User (وقتی صدق می‌کند)

اگر محصول کسی غیر از استفاده‌کننده‌ی نهایی برایش پول می‌دهد (مدل B2B که یک Business بابت داده/تحلیل/ابزار پول می‌دهد ولی End User فقط مصرف‌کننده است)، این تمایز باید از روز اول Blueprint مشخص باشد.
جزئیات مدل‌سازی در `05-B2B-DATA-MODEL.md`.

**تشخیص نقض:** اگر معماری داده طوری طراحی شده که مشخص نیست چه داده‌ای متعلق به کدام طرف است، این قانون نقض شده.

## قانون ۸ — یک محصول در یک زمان

هم‌زمان بیش از یک محصول در فاز Discovery تا MVP ساخته نمی‌شود.
محصول بعدی فقط زمانی شروع می‌شود که محصول فعلی به KPI هدفش رسیده باشد یا آگاهانه متوقف شده باشد — طبق `06-PORTFOLIO-RULES.md`.

**تشخیص نقض:** این قانون در گذشته بیشترین بار نقض شده — شش پروژه‌ی موازی، هیچ‌کدام به مرحله‌ی تست مشتری نرسیده. اگر همزمان روی دو ایده کد می‌نویسی، این قانون در حال نقض شدن است.

## قانون ۹ — یادگیری هر پروژه ثبت می‌شود

هر پروژه (چه موفق چه متوقف‌شده) باید در پایان `07-LEARNING-LOG-TEMPLATE.md` را کامل کند.
بدون این ثبت، تجربه از بین می‌رود و پروژه بعدی دوباره از صفر شروع می‌کند — دقیقاً همان مشکلی که SPF قرار است حل کند.

## قانون ۱۰ — سادگی توضیح

اگر توضیح محصول به یک غریبه بیشتر از ۳۰ ثانیه طول بکشد، محصول بیش از حد پیچیده شده.
این قانون در Blueprint اولیه تست می‌شود، نه بعد از ساخت.

```

</FILE>

---

<FILE path="SPF/02-BLUEPRINT-TEMPLATE.md" tokens="699" lines="92">

```md
# 02 — Blueprint Template

این فرم را قبل از نوشتن اولین خط کد هر محصول تازه پر کن — کامل، حتی اگر بعضی جواب‌ها فعلاً «نمی‌دانم» باشد.
هدف این نیست که فرم زیبا پر شود؛ هدف این است که قبل از کدنویسی، حداقل یک‌بار مجبور شوی به این سؤال‌ها فکر کنی.

اگر پر کردن این فرم بیشتر از ۳۰ دقیقه طول کشید، یا محصول را ساده‌تر کن یا نشانه‌ی این است که هنوز به اندازه‌ی کافی روی ایده فکر نکرده‌ای.

---

## مشخصات محصول

**نام محصول:**

**این محصول دقیقاً چه مشکلی را حل می‌کند؟** (یک جمله، نه یک پاراگراف)

**توضیح ۳۰ ثانیه‌ای برای یک غریبه:**
> اگر این توضیح را با صدای بلند بخوانی و بیشتر از ۳۰ ثانیه طول کشید، طبق قانون ۱۰ Constitution، ساده‌ترش کن.

---

## مخاطب و مدل پول

**چه کسی End User است؟** (کسی که مستقیم از محصول استفاده می‌کند)

**چه کسی Payer است؟** (کسی که پول می‌دهد)

> اگر این دو یکی نیستند → طبق قانون ۷ Constitution، فایل `05-B2B-DATA-MODEL.md` را همین الان پر کن، قبل از ادامه.

**مدل درآمد اولیه (حتی فرضی):** (اشتراک ماهانه؟ به‌ازای هر استفاده؟ یک‌بار پرداخت؟ فریمیوم؟)

**Payer چقدر حاضر است بابت این پول بدهد؟** (یک عدد حدسی هم بهتر از هیچ است — این عدد در میدان تست می‌شود)

---

## فرضیه‌ی اصلی

**فرضیه‌ای که این محصول قرار است تست کند:** (یک جمله به فرمت «اگر X را بسازیم، Y اتفاق می‌افتد»)

**اگر این فرضیه غلط از آب دربیاید، چطور می‌فهمیم؟** (چه رفتاری نشانه‌ی شکست فرضیه است؟)

---

## KPI اصلی

**تنها KPI که این محصول با آن سنجیده می‌شود:** (طبق `04-KPI-FRAMEWORK.md` انتخاب کن — باید Revenue-linked باشد، نه فقط Signup/Usage)

**سقف/هدف این KPI برای عبور به فاز بعد:**

---

## دامنه‌ی MVP (طبق قانون ۳ Constitution — حداکثر ۲ روز ساخت)

**MVP دقیقاً شامل چه چیزهایی است؟** (لیست کوتاه — هرچه کوتاه‌تر بهتر)

-
-
-

**چه چیزهایی عمداً ساخته نمی‌شوند؟** (این بخش مهم‌تر از بخش بالاست — هر چیزی که اینجا نیست یعنی فعلاً حذف شده)

-
-
-

**اگر بعداً دیتابیس/زیرساخت عوض شود، این تصمیم چقدر گران تمام می‌شود؟** (یک برآورد کلی — جزئیات فنی در VibeCoding-STD)

---

## مسیر رسیدن به مشتری (طبق قانون ۴ Constitution — حداکثر ۱ هفته بعد از MVP)

**دقیقاً چه کسانی را در این هفته می‌بینی؟** (اسم/دسته‌ی مشخص، نه «یک نفر پیدا می‌کنم»)

**چطور می‌رسی به آن‌ها؟** (کانال مشخص: حضوری، تلفنی، معرفی از کسی؟)

---

## Reuse Check (طبق قانون ۶ Constitution)

**کدام بخش‌های این محصول زیرساختی هستند (Auth, DB, Payment, ...) و کدام سرویس آماده برایشان انتخاب شده؟**

**کدام بخش واقعاً مزیت رقابتی محصول است و باید از صفر ساخته شود؟**

> این جواب‌ها را همین الان در فایل `08-PROJECT-STATE.md` این محصول (بخش «Foundation انتخاب‌شده») هم ثبت کن — یک‌بار اینجا نوشتن کافی نیست، چون AI در چت بعدی این Blueprint را نمی‌بیند.

---

## تصمیم نهایی قبل از شروع

- [ ] این Blueprint را کامل خواندم و با قوانین `01-CONSTITUTION.md` تضادی ندارد.
- [ ] آماده‌ام این را طبق برنامه در ۲ روز بسازم و در ۱ هفته جلوی مشتری واقعی ببرم.
- [ ] اگر این دو مهلت رد شد، محصول را کوچک‌تر می‌کنم — بزرگ‌ترش نمی‌کنم.

```

</FILE>

---

<FILE path="SPF/03-EVIDENCE-GATES.md" tokens="467" lines="53">

```md
# 03 — Evidence Gates

هر مرحله فقط با شواهد مشخص باز می‌شود، نه با حدس یا ذوق شخصی.
اگر شواهد کافی نیست، برنمی‌گردی به کدنویسی — برمی‌گردی به مرحله‌ی قبل یا محصول را کوچک‌تر می‌کنی.

---

## دروازه‌ی ۱ — از Discovery به MVP

**سؤال:** آیا اصلاً ارزش ساختن نسخه‌ی واقعی‌تر را دارد؟

**Evidence لازم (حداقل یکی، ترجیحاً بیشتر):**
- [ ] حداقل ۳ مکالمه‌ی واقعی با مشتری بالقوه (نه دوست/فامیل) درباره‌ی همین مشکل
- [ ] حداقل یک نفر گفته «الان همین مشکل رو دارم» (نه «شاید یه روز به دردم بخوره»)
- [ ] هیچ گزینه‌ی رایگان/ساده‌تری که همین مشکل را حل کند پیدا نکردی (یا اگر پیدا کردی، دلیل روشنی داری که چرا مال تو بهتر است)

**اگر رد شد:** ایده را کنار بگذار یا مشکل را بازتعریف کن. کدنویسی نکن.

---

## دروازه‌ی ۲ — از MVP به Stabilize & Optimize

**سؤال:** آیا اولین فرضیه (که مردم برایش پول می‌دهند) تأیید شده؟

**Evidence لازم:**
- [ ] حداقل ۱ نفر/کسب‌وکار واقعی، پرداخت واقعی انجام داده یا تعهد کتبی/شفاهی روشن پرداخت داده
- [ ] حداقل ۱ نفر بدون یادآوری تو، دوباره برگشته و استفاده کرده (Retention سیگنال)
- [ ] معیار موفقیتی که در Blueprint نوشته بودی، برآورده شده

**اگر رد شد:**
- اگر هیچ‌کس حتی علاقه نشان نداد → طبق قانون ۱ Constitution، محصول را کوچک‌تر کن.
- اگر علاقه بود ولی پرداخت نبود → قیمت‌گذاری/مدل درآمد را دوباره بررسی کن، نه فیچر اضافه کن.

---

## دروازه‌ی ۳ — از Stabilize به Scale

**سؤال:** آیا محدودیت فنی/عملیاتی واقعی احساس می‌شود؟

**Evidence لازم:**
- [ ] تعداد کاربر/مشتری واقعی از حدی گذشته که مدیریت دستی سخت شده
- [ ] درآمد به‌اندازه‌ای رسیده که هزینه‌ی Downtime یا کندی، واقعاً قابل توجه است
- [ ] حداقل یک مشتری واقعی موضوع کندی/محدودیت را مستقیماً مطرح کرده (نه فرض خودت)

**اگر رد شد:** روی Scale سرمایه‌گذاری نکن؛ روی جذب مشتری بیشتر با همان معماری فعلی تمرکز کن.

---

## قانون کلی هر دروازه

هیچ دروازه‌ای را با «فکر می‌کنم آماده‌ایم» رد نکن.
اگر Evidence روی کاغذ (یا در `07-LEARNING-LOG-TEMPLATE.md`) نوشته نشده، انگار وجود ندارد.

```

</FILE>

---

<FILE path="SPF/04-KPI-FRAMEWORK.md" tokens="487" lines="47">

```md
# 04 — KPI Framework

هر محصول فقط یک KPI اصلی دارد. این فایل کمک می‌کند آن یک عدد را درست انتخاب کنی.

---

## قانون انتخاب KPI

KPI اصلی باید **Revenue-linked** باشد، نه صرفاً Usage یا Engagement.

**چرا:** با فلسفه‌ی خودت («ایده → اولین مشتری پرداخت‌کننده در کمترین زمان»)، اگر KPI فقط تعداد کاربر یا بازدید باشد،
ممکن است محصولی با کاربر زیاد ولی بدون پرداخت‌کننده، اشتباهاً «موفق» به نظر برسد — دقیقاً همان چیزی که در CarIQ اتفاق افتاد (بازی‌ها کامل شدند، تحلیل رفتار مشتری هنوز وصل نشده).

## سلسله‌مراتب KPI (به ترتیب اولویت)

اگر می‌توانی، همیشه KPI را از بالای این لیست انتخاب کن:

1. **Revenue واقعی** (تومان/دلار دریافت‌شده)
2. **تعهد پرداخت مشخص** (پیش‌فاکتور امضاشده، قرارداد، پیش‌پرداخت)
3. **درخواست فعال خرید** (کسی مستقیم پرسیده «چطور بخرم/چقدر می‌شه»)
4. فقط اگر محصول در فاز Discovery محض است: **Signal علاقه‌ی قوی** (لیست انتظار واقعی با اطلاعات تماس، نه فقط لایک)

**هرگز به‌عنوان KPI اصلی استفاده نکن (فقط به‌عنوان KPI فرعی/کمکی قابل قبول‌اند):**
- تعداد بازدید/ثبت‌نام بدون پرداخت
- تعداد کاربرانی که "استفاده کردند" ولی هزینه نداده‌اند
- لایک/اشتراک‌گذاری در شبکه‌ی اجتماعی

## تعریف «مشتری» برای این سیستم

طبق قانون ۹ Constitution (رفتار مهم‌تر از حرف):

> «مشتری» یعنی کسی که حداقل یک تعهد پرداخت واقعی (نه صرفاً ثبت‌نام رایگان) داده است.

## سقف KPI (چه زمانی محصول بعدی شروع می‌شود)

طبق فلسفه‌ی SPF («محصول بعدی وقتی شروع می‌شه که KPI قبلی به سقفش رسیده یا آگاهانه متوقف شده»)،
قبل از شروع هر محصول در Blueprint بنویس: **سقف KPI این محصول چه عددی است که با رسیدن به آن، محصول بعدی را شروع می‌کنم؟**

مثال: «وقتی ماهانه ۲۰ کارت‌ویزیت فروختم و این عدد ۲ ماه ثابت ماند، یعنی یا باید روی رشد سرمایه‌گذاری کنم یا محصول بعدی را شروع کنم.»

## نمونه برای iCard (پیش از تست — فرضی)

- KPI اصلی فرضی: تعداد کسب‌وکارهایی که برای نسخه‌ی آنالیزدار (نه فقط کارت ساده) پول داده‌اند
- KPI فرعی قابل ردیابی: تعداد اسکن QR در هفته (فقط برای فهمیدن رفتار، نه برای قضاوت موفقیت)

> بعد از تست واقعی، این بخش با عدد واقعی جایگزین می‌شود.

```

</FILE>

---

<FILE path="SPF/05-B2B-DATA-MODEL.md" tokens="676" lines="61">

```md
# 05 — B2B Data Model (Payer / Business / End User)

اکثر محصولات این سیستم سه نقش دارند که نباید با هم قاطی شوند. این فایل قبل از طراحی دیتابیس/معماری خوانده شود.

---

## سه نقش

1. **Payer (پرداخت‌کننده):** کسب‌وکاری که هزینه‌ی سرویس را می‌دهد.
2. **Business Owner (صاحب/اپراتور):** کسی که از پنل/داشبورد استفاده می‌کند (معمولاً همان Payer، ولی نه همیشه — مثلاً یک کارمند فروش ممکن است اپراتور باشد ولی صاحب فروشگاه Payer باشد).
3. **End User (کاربر نهایی/مشتری مشتری):** کسی که مستقیماً محصول را لمس می‌کند اما هزینه نمی‌دهد — مثلاً کسی که کارت‌ویزیت را اسکن می‌کند، یا مشتری‌ای که به تعویض‌روغنی مراجعه کرده.

## چرا این تفکیک حیاتی است

اگر این سه نقش را از اول مدل نکنی، وقتی محصول رشد کند این مشکلات پیش می‌آید:

- داده‌ی End User (مثل اطلاعات تماس، رفتار اسکن) باید متعلق به Business باشد، نه به‌صورت عمومی/مشترک ذخیره شود — وگرنه مشکل حریم خصوصی و مالکیت داده پیش می‌آید.
- تغییر ساختار بعد از رشد (مثلاً وقتی بخواهی Multi-tenant کنی) بسیار گران‌تر از تعریف درست از روز اول است.
- بدون این تفکیک، مشخص نیست تحلیل و گزارش‌ها (Analytics) باید حول کدام واحد جمع شوند.

## سؤالاتی که در Blueprint هر محصول باید جواب داده شوند

برای هر محصول B2B:

- [ ] Payer دقیقاً کیست؟
- [ ] آیا Business Owner و Payer یکی هستند یا نه؟
- [ ] End User چه داده‌ای تولید می‌کند؟ (مثال: کلیک، اسکن، موقعیت مکانی، زمان)
- [ ] این داده متعلق به کدام Business است؟ (باید یک شناسه‌ی Business به هر رکورد End User وصل باشد)
- [ ] آیا End User خودش هم اکانت/دسترسی جدا دارد؟ (مثال: Carbook — راننده هم اکانت خودش را دارد و می‌تواند فقط داده‌ی ماشین خودش را ببیند)

## نمونه‌ی مدل‌سازی — iCard

```
Business (Payer + Owner)
  └── دارای یک یا چند Card
       └── هر Card دارای Analytics Events (مستقل، فقط قابل مشاهده توسط همان Business)
            ├── ScanEvent { کجا، کی، چه دستگاهی }
            ├── LinkClickEvent { کدام لینک، چه زمانی }
            └── (End User در این مدل معمولاً هیچ اکانتی ندارد — فقط منبع رویداد است)
```

## نمونه‌ی مدل‌سازی — Carbook (تعویض روغن)

```
Business (تعویض‌روغنی) — Payer + Owner
  └── دارای Customers (رانندگان) که در سیستم او ثبت شده‌اند
       └── هر Customer دارای Car
            └── هر Car دارای Service Records (تاریخچه‌ی تعویض روغن)

Driver (End User) — می‌تواند اکانت جدا داشته باشد
  └── فقط به Service Records ماشین خودش دسترسی دارد
  └── این Service Record ها می‌توانند از چند Business مختلف آمده باشند
```

توجه: اینجا برخلاف iCard، End User (راننده) واقعاً اکانت و دسترسی جدا دارد — پس مدل داده متفاوت است.
این تفاوت را باید در Blueprint هر محصول صریحاً مشخص کرد، نه یک الگوی واحد را روی همه پیاده کرد.

## قانون طلایی این فایل

هیچ رکورد End User نباید بدون شناسه‌ی Business ذخیره شود، مگر اینکه محصول صراحتاً B2C باشد (که طبق فلسفه‌ی SPF، این حالت استثناست نه پیش‌فرض).

```

</FILE>

---

<FILE path="SPF/06-PORTFOLIO-RULES.md" tokens="447" lines="46">

```md
# 06 — Portfolio Rules

قوانین مدیریت چند محصول برای جلوگیری از پخش‌شدن تمرکز — دقیقاً مشکلی که در سابقه‌ی پروژه‌های قبلی (۶ پروژه‌ی هم‌زمان نیمه‌کاره) دیده شد.

---

## قانون اصلی

**هم‌زمان فقط یک محصول در فاز فعال (Discovery تا Stabilize) وجود دارد.**

محصول دوم فقط زمانی شروع می‌شود که محصول اول یکی از این دو حالت را داشته باشد:
- به سقف KPI خودش رسیده (طبق `04-KPI-FRAMEWORK.md`)، یا
- آگاهانه و مکتوب متوقف شده (با `07-LEARNING-LOG-TEMPLATE.md` پر‌شده)

## چرا این قانون برای وضعیت فعلی حیاتی است

نگاهی به وضعیت قبلی: CarIQ، کارت ویزیت هوشمند، کارت عروسی، Carbook، Memorial، قراردادیار — همه هم‌زمان در ذهن/کد وجود داشتند.
نتیجه: هیچ‌کدام به مرحله‌ی تست واقعی با مشتری نرسید.
این قانون مستقیماً همین را هدف گرفته.

## اگر وسط کار یک ایده‌ی جدید به ذهنت رسید

- [ ] آن را در یک فایل `IDEAS-BACKLOG.md` (خارج از این پوشه) یادداشت کن — همان لحظه، فقط یک خط.
- [ ] به آن دست نزن تا محصول فعلی به یکی از دو حالت بالا برسد.
- [ ] هیچ کدنویسی روی ایده‌ی جدید انجام نشود، حتی «فقط یه POC کوچیک».

**این دقیقاً همان لحظه‌ای است که در گذشته اتفاق افتاده — نوشتن این قانون کافی نیست، رعایتش لحظه‌ی وسوسه سخت‌ترین بخش است.**

## وقتی محصول متوقف می‌شود (نه موفق)

توقف شکست نیست، اگر آگاهانه و با یادگیری مکتوب باشد.
توقفی که "شکست" واقعی است: رها کردن بی‌سروصدا بدون ثبت اینکه چرا، و رفتن سراغ ایده‌ی بعدی بدون یادگیری.

## ترتیب فعلی صف پروژه‌ها (پر کن و به‌روز نگه دار)

| اولویت | محصول | وضعیت | یادداشت |
|---|---|---|---|
| ۱ (فعال) | iCard | در حال تست مشتری | |
| برگشت‌ناپذیر تا اینجا | CarIQ | متوقف — منتظر یادگیری‌لاگ | |
| صف | Carbook | شروع نشده | |
| صف | Memorial | شروع نشده | |
| صف | کارت عروسی | شروع نشده | |
| نگه‌داشته‌شده | قراردادیار | آگاهانه کنار گذاشته شده (طبق خودت) | |

> این جدول را بعد از هر تغییر وضعیت به‌روز کن — این خودش یک‌جور Evidence Gate بصری است.

```

</FILE>

---

<FILE path="SPF/07-LEARNING-LOG-TEMPLATE.md" tokens="342" lines="54">

```md
# 07 — Learning Log Template

این فایل را برای **هر محصول** — چه موفق چه متوقف‌شده — بعد از پایان هر چرخه‌ی تست کامل کن.
بدون این فایل، SPF از تجربه یاد نمی‌گیرد و همان اشتباهات تکرار می‌شوند.

کپی کن و برای هر محصول یک نسخه‌ی جدا نگه دار (مثال: `07-LOG-iCard.md`).

---

## محصول

[نام]

## تاریخ شروع / تاریخ این ثبت

[شروع: ... / ثبت: ...]

## چه چیزی تست شد

[دقیقاً چه نسخه‌ای، جلوی چه کسانی، چطور]

## نتیجه‌ی واقعی (نه برداشت، عدد/اتفاق واقعی)

- تعداد افرادی که واقعاً دیدند: 
- تعداد افرادی که واکنش مثبت واقعی نشان دادند (طبق تعریف قانون ۹ Constitution): 
- تعداد پرداخت/تعهد واقعی: 
- آیا دروازه‌ی Evidence مربوطه (`03-EVIDENCE-GATES.md`) رد شد یا قبول؟

## چه چیزی درست بود

[حتی اگر محصول متوقف شد، چه بخشی از فرض/طراحی درست از آب درآمد]

## چه چیزی اشتباه بود

[دقیق باش — کجای فرض اشتباه بود، نه فقط «بازار نخواست»]

## کدام فرضیه رد شد

[مثال: فرض کرده بودم کسب‌وکارهای کوچک برای آنالیز کارت‌ویزیت پول می‌دهند — رد شد چون ...]

## تصمیم نهایی

- [ ] ادامه به فاز بعد (Evidence Gate رد شد)
- [ ] کوچک‌تر کردن و تست دوباره
- [ ] توقف کامل (آگاهانه)

## چه چیزی باید وارد Foundation/VibeCoding-STD شود

[اگر یک تصمیم فنی یا Prompt خاص خوب جواب داد، اینجا بنویس تا در پروژه‌ی بعدی از صفر تکرار نشود]

## چه چیزی باید از SPF یا Constitution اصلاح شود

[اگر یکی از قوانین SPF در عمل دست‌وپاگیر یا اشتباه بود، اینجا بنویس — این ورودی مستقیم نسخه‌ی بعدی SPF است]

```

</FILE>

---

<FILE path="SPF/08-PROJECT-STATE.md" tokens="403" lines="58">

```md
# 08 — Project State

این فایل «حافظه‌ی زنده‌ی پروژه» است — چیزی که چت جدید با AI از آن بی‌خبر است.
بدون این فایل، AI در هر چت تازه پروژه را از صفر می‌بیند: ممکن است Foundation را دوباره بسازد،
تصمیمی را نقض کند که قبلاً آگاهانه گرفته شده، یا Entity را جوری مدل کند که با بقیه‌ی پروژه ناسازگار باشد.

کپی کن و برای هر محصول یک نسخه‌ی جدا نگه دار (مثال: `08-STATE-iCard.md`).
این فایل **همراه `01-CONSTITUTION.md` در ابتدای هر چت جدید** به AI داده شود.

قانون طلایی این فایل: کوتاه بماند. اگر یک بخش دارد پاراگراف می‌شود، جای درستش کد یا مستندات فنی است، نه اینجا.
هر تصمیم تازه که گرفته می‌شود، همان لحظه یک خط اینجا اضافه شود — نه در پایان پروژه.

---

## محصول

[نام]

## Foundation انتخاب‌شده

فقط یک خط برای هرکدام — چه سرویس/کتابخانه انتخاب شده، نه جزئیات پیاده‌سازی:

| نیاز | انتخاب شده | تاریخ تصمیم |
|---|---|---|
| Authentication | | |
| Database / ORM | | |
| Storage | | |
| Billing | | |
| Analytics | | |
| Notification (Email/SMS) | | |
| AI Provider | | |
| (هر مورد دیگر) | | |

> اگر نیازی هنوز تصمیم‌گیری نشده، خالی بگذار — نه اینکه حدس بزنی.

## تصمیم‌های معماری مهم + دلیل

فقط یک خط دلیل، نه پاراگراف. هدف این است که ۶ ماه بعد کسی نپرسد «چرا این را انتخاب کردیم؟».

- چرا [Prisma/Drizzle/...]: 
- چرا [Supabase/...]: 
- چرا [Repository Pattern/...]: 
- چرا [...]: 

## Entity های اصلی

فقط اسم + یک جمله. Schema کامل جای خودش در کد است، نه اینجا.

| Entity | یک‌جمله توضیح | متعلق به کدام Business/Owner است؟ |
|---|---|---|
| مثال: Customer | | |
| مثال: Order | | |

## آخرین وضعیت فاز

فاز فعلی طبق `02-PHASES.md`: [Discovery / MVP / Growth / Scale]

آخرین به‌روزرسانی این فایل: [تاریخ]
```

</FILE>

---

<FILE path="SPF/README.md" tokens="628" lines="63">

```md
# SPF — Solo Product Factory (V1)

این پوشه سیستم کاری من برای تبدیل ایده به کسب‌وکار واقعی است — نه فقط ساخت نرم‌افزار.

## هدف SPF

جلوگیری از تکرار الگویی که در پروژه‌های قبلی افتاد:

> ایده → کدنویسی کامل و ایده‌آل‌گرایانه → هیچ‌وقت تست با مشتری واقعی → پروژه بعدی

الگوی درست:

> ایده → Discovery → Evidence → Blueprint → MVP → Evidence → Stabilize → Evidence → Scale

در پایان هر مرحله فقط یک سؤال مهم است: **آیا شواهد کافی برای رفتن به مرحله بعد داریم؟**
اگر نه، برنمی‌گردیم به کدنویسی بیشتر — برمی‌گردیم به مرحله قبل یا محصول را کوچک‌تر می‌کنیم.

## SPF چیست و چه چیزی نیست

**هست:**
- چارچوب تصمیم‌گیری برای اینکه چه محصولی بسازیم و چه زمانی متوقف/ادامه بدهیم.
- سیستمی که تجربه هر پروژه را به پروژه بعدی منتقل می‌کند.

**نیست:**
- استاندارد فنی کدنویسی (آن در Repository جدا `VibeCoding-STD` است).
- یک متدولوژی سنگین مدیریت محصول با جلسات و مراسم تیمی — این برای یک نفر است.
- بهانه‌ای برای تعویق افتادن رفتن سراغ مشتری واقعی.

## تفاوت SPF با VibeCoding-STD

| | SPF | VibeCoding-STD |
|---|---|---|
| سؤال اصلی | چه چیزی بسازیم؟ برای چه کسی؟ چرا؟ | چطور بسازیم؟ |
| واحد کار | محصول / فرضیه / Evidence | Feature / Sprint / کد |
| وقتی استفاده می‌شود | قبل از کد، بین فازها، پایان پروژه | حین کدنویسی |

هر پروژه هر دو را همزمان لازم دارد. SPF تصمیم می‌گیرد؛ STD اجرا می‌کند.

## ترتیب استفاده

1. **ایده‌ی تازه** → `01-CONSTITUTION.md` را مرور کن؛ ببین با قوانین ثابت جور در می‌آید یا نه.
2. **قبل از هر خط کد** → `02-BLUEPRINT-TEMPLATE.md` را پر کن.
3. **در پایان هر فاز** → `03-EVIDENCE-GATES.md` را چک کن؛ فقط با Evidence کافی وارد فاز بعد شو.
4. **قبل از تعیین KPI محصول** → `04-KPI-FRAMEWORK.md` را ببین.
5. **اگر محصول B2B با کاربر نهایی جدا از پرداخت‌کننده است** → `05-B2B-DATA-MODEL.md` را پر کن.
6. **قبل از شروع محصول بعدی** → `06-PORTFOLIO-RULES.md` را چک کن.
7. **پایان هر پروژه (موفق یا متوقف‌شده)** → `07-LEARNING-LOG-TEMPLATE.md` را کامل کن.

## قانون طلایی

> اگر واقعیت با این سند مغایرت داشت، مشکل از پروژه توست، نه از سند.
> اما اگر سند در میدان دست‌وپاگیر یا غیرواقعی بود، خودِ سند را اصلاح کن.

این سند فقط با تجربه‌ی واقعی اصلاح می‌شود، نه با فکر کردن بیشتر درباره‌اش.

## نسخه‌بندی

- **V1 (فعلی):** حداقلی. بر مبنای تحلیل چند پروژه‌ی قبلی (CarIQ، کارت ویزیت هوشمند، Carbook، Memorial، قراردادیار) که هیچ‌کدام به مرحله‌ی تست مشتری واقعی نرسیدند.
- **V2:** بعد از این‌که حداقل یک محصول (iCard) واقعاً جلوی چند مشتری واقعی رفت و Evidence واقعی جمع شد.
- **V3:** بعد از تکرار این چرخه روی چند محصول.

هیچ فایلی در این نسخه کامل یا نهایی نیست — همه باید بعد از تست iCard اصلاح شوند.

```

</FILE>

---

<FILE path="VibeCoding-STD/01-CONSTITUTION.md" tokens="1022" lines="100">

```md
# 01 — Constitution

قوانین این فایل **در تمام فازها** (POC تا Scale) بدون استثنا اعمال می‌شوند.
اگر جایی نیاز به نقض یکی از این قوانین احساس شد، آن نقض باید آگاهانه و مستند باشد، نه ناخواسته.

این فایل باید در ابتدای هر پروژه/چت جدید به AI داده شود.

---

## قانون ۱ — Reuse First (اول استفاده، بعد ساخت)

قبل از نوشتن هر قابلیت جدید، AI باید به این ترتیب بررسی کند:

1. آیا این قابلیت در خودِ Framework وجود دارد؟
2. آیا یک سرویس/پلتفرم آماده و معتبر برای آن هست؟ (مثل Supabase Auth, Clerk, Cloudinary, S3)
3. آیا کتابخانه استاندارد و پرکاربردی برایش هست؟
4. آیا قبلاً در همین پروژه پیاده‌سازی شده؟
5. فقط اگر پاسخ همه موارد بالا «خیر» بود، کد جدید نوشته شود.

**ممنوع:** ساخت دوباره‌ی Auth، Billing، RBAC، Storage، QR Generator یا هر ماژول زیرساختی رایج، بدون بررسی گزینه‌های آماده.
**استثنا:** فقط چیزی که مزیت رقابتی واقعی محصول است (مثل منطق اختصاصی AI، الگوریتم خاص، Workflow منحصر) حق دارد از صفر نوشته شود.

## قانون ۲ — یک منبع داده برای هر Entity (One Source of Truth)

هر Entity (مثل Customer، Order، Product) فقط از یک مسیر خوانده و نوشته می‌شود — معمولاً یک Repository مشخص.

**ممنوع:** ترکیب هم‌زمان localStorage + آرایه داخلی + fetch برای یک Entity واحد.
**تشخیص خطا:** اگر برای پیدا کردن «نسخه‌ی درست» داده مجبور شدی چند فایل را بگردی، این قانون نقض شده.

## قانون ۳ — همه‌چیز موقت باید برچسب بخورد (Label Everything)

هر داده یا منطق موقت (Mock، Hardcoded، LocalStorage placeholder) باید علامت‌گذاری شود:

```
// TODO_REMOVE_BEFORE_DATABASE
// TEMP DATA
```

و بالای هر فایل که با داده سروکار دارد، این برچسب باید باشد:

```
Data Source: Database | LocalStorage | Mock | Hardcoded
```

**دلیل:** بدون این برچسب، موقتی‌ها فراموش شده و وارد نسخه واقعی می‌شوند.

## قانون ۴ — معماری قبل از کد (Architecture Before Code)

AI حق ندارد بدون توضیح، تصمیم معماری بگیرد (اینکه داده کجا ذخیره شود، چطور جریان پیدا کند).
قبل از نوشتن کد برای هر Feature تازه، AI باید Data Flow آن را به‌صورت خلاصه توضیح دهد:

```
UI → Service → Repository → Database
```

اگر مسیر داده مستقیم UI → Database (بدون Service/Repository) بود، یا Analytics مستقیم از UI/localStorage خوانده می‌شد، این قانون نقض شده است.

علاوه بر Data Flow، قبل از نوشتن کد هر Feature، AI باید این تصمیم‌ها را صریح اعلام کند: منبع داده (Data Source)، Repository، Caching، Permission، Validation، سرویس‌های خارجی (External Services)، هر Dependency تازه.
اگر یکی از این‌ها بدون اعلام قبلی در کد ظاهر شود، این قانون نقض شده است. پرامپت آماده در `06-PROMPTS.md`.

## قانون ۵ — بدون Secret در Frontend

هیچ کلید API، توکن یا Secret نباید داخل کد Frontend یا Repository عمومی قرار بگیرد.
همه باید در Environment Variables سمت سرور باشند.

## قانون ۶ — بدون عدد یا قانون تجاری هاردکد (No Magic Numbers / Business Rules)

مقادیری مثل نرخ مالیات، درصد تخفیف، سقف تعداد، role admin و مشابه آن، باید در Configuration باشند نه داخل کد.

```
// اشتباه
const TAX = 9;

// درست
const TAX = config.tax;
```

## قانون ۷ — قطعیت و تست‌پذیری (Determinism & Testability)

منطق تجاری (Business Logic) باید:
- از UI/Component جدا و به‌صورت تابع مستقل نوشته شود، حتی اگر فعلاً تستی برایش نباشد.
- به `Math.random()`، `Date.now()`، یا مقدار DOM مستقیم وابسته نباشد — این‌ها باید به‌عنوان ورودی/پارامتر پاس داده شوند.
- Dependency (مثل Repository) از بیرون به تابع تزریق شود، نه اینکه تابع خودش مستقیم `localStorage`/`fetch` را صدا بزند.

**دلیل:** حتی اگر الان تست ننویسی، این قوانین مسیر تست‌پذیری را برای آینده باز نگه می‌دارند. جزئیات الزام تست به فاز، در `02-PHASES.md` آمده.

## قانون ۸ — وابستگی باید دلیل داشته باشد (No Dependency Chaos)

برای هر کار، فقط یک کتابخانه انتخاب شود (نه axios + fetch + ky هم‌زمان برای یک کار).
اگر AI کتابخانه‌ی دومی برای همان منظور پیشنهاد داد، باید دلیل جایگزینی کتابخانه‌ی قبلی را توضیح دهد.

## قانون ۹ — مستندسازی کوتاه هر Feature

هر Feature تازه باید یک توضیح چندخطی داشته باشد: داده از کجا می‌آید، کجا ذخیره می‌شود، چه کسی مصرفش می‌کند. جزئیات این سؤال‌ها در `05-CHECKLIST.md` است.

## قانون ۱۰ — بدون شکست خاموش (No Silent Failure)

هر مسیری که می‌تواند خطا بدهد (fetch، محاسبه، پارس داده) باید حالت Error و Empty State داشته باشد.
**ممنوع:** نمایش نتیجه‌ی اشتباه بدون هیچ Error یا هشدار قابل مشاهده.

```

</FILE>

---

<FILE path="VibeCoding-STD/02-PHASES.md" tokens="626" lines="88">

```md
# 02 — Phases

استاندارد باید متناسب با فاز پروژه سبک یا سنگین شود. قوانین `01-CONSTITUTION.md` در همه فازها ثابت‌اند؛
این فایل مشخص می‌کند در هر فاز چه چیزی **مجاز**، چه چیزی **ممنوع**، و **معیار خروج** به فاز بعد چیست.

قبل از شروع کار روی پروژه، مشخص کن الان در کدام فاز هستی و همان بخش را به AI بده.

---

## فاز ۱ — Discovery / POC

**هدف:** فقط اثبات ایده. هیچ‌کس واقعی هنوز از این استفاده نمی‌کند.

**مجاز:**
- Mock Data، LocalStorage، Fake API
- Authentication ساده یا حتی بدون Auth
- بدون Cache، بدون Queue، بدون Microservice

**ممنوع:**
- هیچ‌کدام از موارد بالا بدون برچسب (طبق قانون ۳ Constitution)

**معیار خروج به MVP:**
- ایده اعتبارسنجی شده (حداقل یک نفر غیر از خودت آن را دیده و تأیید کرده)
- تصمیم گرفته شده که پروژه ارزش ساخت واقعی دارد

---

## فاز ۲ — MVP

**هدف:** کاربر واقعی از آن استفاده می‌کند.

**دیگر مجاز نیست:**
- Analytics هاردکد یا محاسبه‌شده از DOM
- Business Logic داخل UI/Component
- چند منبع داده برای یک Entity

**الزامی می‌شود:**
- الگوی Repository و Service (حتی اگر Repository هنوز از LocalStorage استفاده کند)
- تست واحد برای منطق تجاری حیاتی (مثل محاسبه قیمت، مالیات، تخفیف)
- مستندسازی کوتاه هر Feature طبق قانون ۹

**معیار خروج به Growth:**
- تعداد کاربر واقعی از یک آستانه مشخص عبور کرده (خودت عدد را برای هر پروژه تعیین کن)
- حداقل یک بار داده واقعی (نه Mock) در مسیر اصلی محصول جریان داشته

---

## فاز ۳ — Growth

**هدف:** محصول باید بدون نظارت مداوم دستی، پایدار بماند.

**باید اضافه شود:**
- Logging و Monitoring
- Error Tracking
- Rate Limiting
- Permission واقعی (نه ظاهری — طبق قانون Authentication در Antipatterns)
- Migration و Backup منظم دیتابیس
- Cache در نقاط پرترافیک
- Background Jobs برای کارهای سنگین/زمان‌بر

**معیار خروج به Scale:**
- محدودیت فنی واقعی حس شده (کندی، صف، نیاز به مقیاس افقی)
- درآمد/کاربر به حدی رسیده که هزینه Downtime قابل توجه است

---

## فاز ۴ — Scale

**هدف:** رشد بدون شکستن.

**باید اضافه شود:**
- Queue و Event-Driven Architecture
- Horizontal Scaling
- CDN و Object Storage
- Feature Flags
- Distributed Cache
- Observability کامل (Trace + Metric + Log یکپارچه)
- Audit Log
- Multi-Tenant (در صورت نیاز مدل کسب‌وکار) و اگر محصول از همان اول چند کاربره است آن را در همان MVP لحاظ کن.

---

## قاعده کلی بین فازها

هیچ‌وقت مستقیم از Discovery به Growth نپر — MVP نباید حذف شود، چون همان جایی است که Repository Pattern و جداسازی Logic شکل می‌گیرد و مهاجرت بعدی را ارزان می‌کند.

اگر پاسخ به «اگر دیتابیس عوض شود چند فایل باید تغییر کند؟» بیشتر از ۲ فایل شد، فاز فعلی درست پیاده نشده — به `05-CHECKLIST.md` مراجعه کن.

```

</FILE>

---

<FILE path="VibeCoding-STD/03-REUSE-FIRST.md" tokens="653" lines="46">

```md
# 03 — Reuse First

طبق قانون ۱ در `01-CONSTITUTION.md`، قبل از نوشتن هر ماژول زیرساختی، باید گزینه‌های آماده بررسی شوند.
این فایل نقطه شروع آن بررسی است — لیست کامل و همیشه‌به‌روز نیست، اما یادآوری می‌کند که کجا نباید از صفر کد نوشت.

هر بار قبل از استفاده، وضعیت گزینه‌ها را با یک جست‌وجوی سریع تأیید کن؛ این حوزه سریع تغییر می‌کند.

---

| نیاز | اول این را بررسی کن | چه زمانی خودت بسازی |
|---|---|---|
| Authentication | Supabase Auth، Clerk، Auth0، Firebase Auth، Better Auth | فقط اگر نیاز به منطق سفارشی خیلی خاص باشد که هیچ‌کدام پشتیبانی نمی‌کند |
| Authorization / RBAC | امکانات داخلی فریم‌ورک، CASL، Permit.io | فقط اگر مدل دسترسی خیلی غیرمعمول است |
| Storage / Upload فایل | S3، Cloudinary، Supabase Storage | تقریباً هیچ‌وقت لازم نیست خودت بنویسی |
| Billing / Subscription | Stripe، Paddle، LemonSqueezy | فقط منطق تجاری خاص روی بالای آن‌ها |
| Database / ORM | Supabase، PostgreSQL + Prisma/Drizzle | — |
| Analytics محصول | PostHog، Plausible، Mixpanel | فقط اگر Analytics خودِ محصول است (مزیت رقابتی) |
| Notification (Email/SMS) | Resend، SendGrid، Kavenegar (برای ایران) | تقریباً هیچ‌وقت |
| QR / Barcode | کتابخانه‌های استاندارد موجود (qrcode.js و مشابه) | تقریباً هیچ‌وقت |
| Error Tracking | Sentry | — |
| Logging / Monitoring | Better Stack، Datadog، خدمات هاست (Liara/Arvan) | فقط تنظیمات سفارشی روی این‌ها |
| CI/CD | GitHub Actions، پلتفرم هاست | — |
| Date/Time handling | یک کتابخانه ثابت انتخاب کن (مثل date-fns) و همان‌جا بمان | هیچ‌وقت خودت الگوریتم تاریخ ننویس |
| Search | Algolia، Typesense، Meilisearch | فقط اگر منطق رتبه‌بندی خیلی خاص محصول است |
| AI Provider | OpenAI، Anthropic، Google، یا Wrapper آماده (Vercel AI SDK) | فقط منطق Prompt/Workflow اختصاصی محصول |
| Workflow / Automation | n8n، Zapier، Make | فقط اگر Workflow واقعاً منحصربه‌فرد محصول است |
| Queue / Background Jobs | سرویس هاست (مثل Supabase Edge Functions + Cron)، BullMQ، Inngest | تقریباً هیچ‌وقت خودت صف بنویس |

---

## چیزی که همیشه خودت می‌سازی (مزیت رقابتی)

این‌ها استثنای قانون Reuse First‌اند، چون هویت محصول تو هستند:

- منطق اختصاصی AI / Agent مربوط به محصول به جز وقتی که از n8n استفاده میکنی (هنگام استفاده از n8n بپرس آیا community nodes آماده هست یا فایل workflow.json آماده یا مسابه وجود دارد؟
- Workflow اختصاصی کسب‌وکار
- ساختار داده و منطق خاص محصول (مثل Customer Vault، بازی سفارشی)
- رابط کاربری و تجربه کاربری

## الگوی بررسی سریع (پیش از هر Feature)

1. نیاز را در یک جمله بنویس.
2. یک جست‌وجوی سریع بزن: `"[نیاز] service OR library 2026"`.
3. اگر گزینه معتبر و پرکاربرد پیدا شد → استفاده کن، فقط تنظیمش کن.
4. اگر نه → طبق قانون ۱ Constitution، فقط در این حالت کد جدید بنویس.

```

</FILE>

---

<FILE path="VibeCoding-STD/04-ANTIPATTERNS.md" tokens="859" lines="61">

```md
# 04 — Antipatterns

لیست الگوهای خطرناک رایج در Vibe Coding. هر مورد: **علامت هشدار** (چطور تشخیص بدهی) و **چرا خطرناک است**.
این فایل را وقتی شک داری («این کد مشکوک به نظر می‌رسد ولی مطمئن نیستم چرا») مرور کن.

---

## ۱. معماری چندمنبعی
**علامت:** برای یک Entity، هم `localStorage`، هم آرایه‌ی محلی، هم `fetch` دیده می‌شود.
**چرا خطرناک:** هیچ‌کس نمی‌داند کدام نسخه‌ی داده «درست» است؛ هنگام مهاجرت، باگ‌های ناسازگار پیدا می‌شوند.

## ۲. State Spaghetti
**علامت:** یک اطلاعات (مثل کاربر لاگین‌شده) در چند جای مختلف نگه‌داری می‌شود — Context، localStorage، URL، متغیر global.
**چرا خطرناک:** به‌روزرسانی یکی، بقیه را sync نمی‌کند؛ باگ‌های ناپدید و سخت-پیدا تولید می‌کند.

## ۳. Mockهای فراموش‌شده
**علامت:** `const users = [...]`، `Math.random()` برای ID، اعداد ثابت برای دموی داشبورد، بدون هیچ برچسبی.
**چرا خطرناک:** بی‌سروصدا وارد نسخه‌ی واقعی می‌شوند و کسی متوجه نمی‌شود تا شکایت کاربر برسد.
**راه تشخیص:** جست‌وجوی `TODO_REMOVE_BEFORE_DATABASE` باید همه‌ی این موارد را نشان دهد. اگر چیزی هست که این برچسب را ندارد، مشکوک است.

## ۴. Happy Path Coding
**علامت:** کد فرض می‌کند اینترنت همیشه وصل، دیتابیس همیشه پاسخگو، کاربر همیشه ورودی درست می‌دهد.
**چرا خطرناک:** در دنیای واقعی هیچ‌کدام همیشه درست نیست؛ نتیجه یک صفحه سفید بدون توضیح برای کاربر است.
**راه تشخیص:** برای هر fetch/محاسبه بپرس: «اگر این失敗 (خطا داد) چه می‌شود؟» اگر پاسخ روشنی نداری، این الگو وجود دارد.

## ۵. Authentication ظاهری
**علامت:** صفحه Login هست، اما Route محافظت نشده، API بدون بررسی توکن، Role چک نمی‌شود.
**چرا خطرناک:** با تغییر مستقیم URL، کاربر عادی وارد صفحه Admin می‌شود.
**راه تشخیص:** یک URL محافظت‌شده را بدون لاگین یا با کاربر سطح پایین امتحان کن؛ باید رد شود.

## ۶. Database Time Bomb
**علامت:** بدون Index، بدون Migration مشخص، همه‌چیز در یک جدول تخت.
**چرا خطرناک:** پروژه با چند صد رکورد خوب کار می‌کند، بعد از چند هزار رکورد به‌شدت کند می‌شود.

## ۷. Context Rot
**علامت:** فایل‌های خیلی بزرگ (بیش از ۲۰۰-۳۰۰ خط)، ساختار غیرماژولار.
**چرا خطرناک:** وقتی پروژه بزرگ می‌شود، AI دیگر همه‌ی فایل‌های مرتبط را در Context ندارد؛ هر اصلاح، جای دیگری را می‌شکند.
**راه تشخیص:** اگر یک فایل بیش از ۳۰۰ خط شده، وقت تقسیم آن است.

## ۸. Prompt Regression (چرخه‌ی شکستن متوالی)
**علامت:** رفع باگ A باعث بروز باگ B می‌شود، رفع B باعث بروز C.
**چرا خطرناک:** نشانه این است که AI معماری کلی را در نظر نمی‌گیرد، فقط آخرین درخواست را حل می‌کند.
**راه تشخیص:** اگر ۲ بار پشت‌سرهم این چرخه رخ داد، به‌جای ادامه‌ی Fix، از AI بخواه Data Flow کامل را دوباره نشان دهد (طبق `06-PROMPTS.md`).

## ۹. Dependency Chaos
**علامت:** چند کتابخانه برای یک کار مشابه (axios + fetch + ky، یا چند کتابخانه تاریخ).
**چرا خطرناک:** حجم باندل بالا می‌رود، رفتار ناسازگار بین کتابخانه‌ها بروز می‌کند.

## ۱۰. Secret Leak
**علامت:** کلید API یا توکن مستقیم در کد Frontend یا در Repository عمومی.
**چرا خطرناک:** یکی از رایج‌ترین و خطرناک‌ترین اشتباهات؛ کلید می‌تواند فوراً سوءاستفاده شود.

## ۱۱. Hardcoded Business Rules
**علامت:** درصد مالیات، تخفیف، سقف‌های عددی مستقیم در کد.
**چرا خطرناک:** هر تغییر قانون تجاری نیاز به Deploy مجدد دارد؛ ریسک خطای انسانی بالا می‌رود.

## ۱۲. Silent Failure (خطرناک‌ترین مورد)
**علامت:** برنامه بدون Error اجرا می‌شود اما نتیجه‌ی محاسباتی اشتباه تولید می‌کند (مثلاً عدد فروش غلط بدون هیچ هشدار).
**چرا خطرناک:** چون هیچ نشانه‌ای ندارد، ممکن است ماه‌ها کشف نشود و تصمیم‌های تجاری غلط بر اساس آن گرفته شود.
**راه تشخیص:** هر مسیر محاسباتی حیاتی باید حداقل یک تست واحد ساده داشته باشد که با داده‌ی شناخته‌شده، نتیجه‌ی شناخته‌شده تولید کند.

```

</FILE>

---

<FILE path="VibeCoding-STD/05-CHECKLIST.md" tokens="636" lines="69">

```md
# 05 — Checklist

این چک‌لیست را در دو زمان اجرا کن:
1. **پایان هر Sprint** (یا هر جلسه‌ی کاری بلند با AI)
2. **قبل از حرکت از یک فاز به فاز بعد** (طبق `02-PHASES.md`)

هدف: پیدا کردن مشکلات قبل از اینکه پروژه بزرگ‌تر و هزینه‌ی اصلاح بالاتر برود.

---

## بخش الف — چهار سؤال برای هر Feature

برای هر قابلیتی که این Sprint اضافه شده، این چهار سؤال را جواب بده:

- [ ] داده از کجا می‌آید؟
- [ ] کجا ذخیره می‌شود؟
- [ ] چه کسی (کدام بخش) آن را مصرف می‌کند؟
- [ ] اگر دیتابیس عوض شود، چند فایل باید تغییر کند؟

> اگر پاسخ سؤال آخر بیشتر از ۲ فایل بود، معماری این Feature ضعیف است — قبل از ادامه، Repository آن را اصلاح کن.

## بخش ب — بررسی برچسب‌ها و موقتی‌ها

- [ ] جست‌وجوی `TODO_REMOVE_BEFORE_DATABASE` و `TEMP DATA` انجام شد و لیست کامل موقتی‌ها مشخص است.
- [ ] بالای هر فایل داده‌محور، برچسب `Data Source: ...` وجود دارد.
- [ ] هیچ Mock بدون برچسب باقی نمانده.

## بخش ج — بررسی معماری

- [ ] هر Entity فقط یک Repository/منبع داده دارد (قانون ۲ Constitution).
- [ ] Business Logic داخل Component/UI نوشته نشده.
- [ ] Analytics مستقیم از localStorage/UI نمی‌خواند، از طریق Service/Repository عبور می‌کند.
- [ ] هیچ فایلی بیش از ۳۰۰ خط نشده (Context Rot).

## بخش د — امنیت و پایداری

- [ ] هیچ Secret/کلید API در Frontend یا Repository عمومی نیست.
- [ ] Route‌های حساس (Admin و مشابه) با کاربر غیرمجاز تست شده و رد می‌شوند.
- [ ] برای مسیرهای اصلی (fetch، محاسبه) حالت Error و Empty State وجود دارد.

## بخش ه — تست‌پذیری (طبق قانون ۷ Constitution)

- [ ] منطق تجاری حیاتی (قیمت، مالیات، تخفیف و مشابه) از UI جدا و به‌صورت تابع مستقل نوشته شده.
- [ ] این توابع به `Math.random()`/`Date.now()`/DOM مستقیم وابسته نیستند.
- [ ] (از فاز MVP به بعد) حداقل یک تست واحد برای هر مسیر محاسباتی حیاتی وجود دارد.

## بخش و — Reuse Check

- [ ] هیچ ماژول زیرساختی (Auth، Storage، Billing، RBAC) بدون بررسی گزینه‌های `03-REUSE-FIRST.md` از صفر نوشته نشده.
- [ ] هیچ دو کتابخانه‌ی هم‌کاره برای یک منظور مشترک نصب نشده.

---

## بخش ز — تکمیل بودن Feature (Feature Complete)

قبل از اینکه یک Feature را «تمام‌شده» اعلام کنی، این‌ها را جداگانه چک کن — «کار می‌کند» با «کامل است» فرق دارد:

- [ ] Loading State دارد
- [ ] Error State دارد
- [ ] Empty State دارد (وقتی داده‌ای نیست)
- [ ] Permission/دسترسی چک شده
- [ ] در موبایل/صفحه کوچک درست نمایش داده می‌شود (Responsive)
- [ ] حداقل موارد پایه Accessibility رعایت شده (label روی input، contrast قابل خواندن)

## اگر این چک‌لیست رد شد

مشکلات پیداشده را در یک لیست کوتاه بنویس و قبل از افزودن Feature تازه، اول همان‌ها را اصلاح کن.
تکرار همین چک‌لیست بدون اصلاح موارد قبلی، فقط بدهی فنی را انباشته می‌کند.

```

</FILE>

---

<FILE path="VibeCoding-STD/06-PROMPTS.md" tokens="688" lines="77">

```md
# 06 — Prompts

پرامپت‌های آماده برای هر مرحله. به‌جای نوشتن دستور از صفر، این‌ها را کپی و تنظیم کن.
همه‌ی این پرامپت‌ها فرض می‌کنند فایل `01-CONSTITUTION.md` قبلاً در همان مکالمه به AI داده شده.

---

## شروع پروژه جدید

```
این قوانین (فایل Constitution پیوست) و وضعیت فعلی پروژه (فایل 08-PROJECT-STATE پیوست) را در تمام این پروژه رعایت کن.
پروژه فعلاً در فاز [Discovery/MVP/Growth/Scale] است — قوانین همان فاز از فایل Phases را هم اعمال کن.
قبل از نوشتن هر کد، معماری Data Flow آن Feature را در یک خط نشان بده:
UI → Service → Repository → Database
اگر جایی مجبور به استفاده از Mock/LocalStorage/Hardcode شدی، آن را با برچسب مشخص کن و دلیلش را بگو.
```

## قبل از هر Feature تازه

```
قبل از نوشتن این Feature، این سؤال‌ها را جواب بده:
۱. آیا این قابلیت آماده (در Framework/سرویس/کتابخانه) وجود دارد؟ (طبق اصل Reuse First)
۲. Data Flow این Feature چیست؟
۳. تصمیم‌های زیر را صریح اعلام کن: Data Source، Repository، Caching، Permission، Validation، External Services، هر Dependency تازه.
۴. اگر بعداً دیتابیس عوض شود، این Feature چند فایل باید تغییر کند؟
بعد از پاسخ به این سؤال‌ها، کد را بنویس.
```

## بررسی معماری فعلی (Data Flow کامل)

```
معماری فعلی پروژه را نشان بده:
- لیست کامل منابع داده (Database, LocalStorage, Mock, Hardcoded) و اینکه هرکدام کجا استفاده شده‌اند.
- Data Flow کامل برای هر Entity اصلی.
- هر جایی که یک Entity بیش از یک منبع داده دارد را مشخص کن.
```

## پیدا کردن موقتی‌های فراموش‌شده

```
تمام کدهایی که برچسب TODO_REMOVE_BEFORE_DATABASE، TEMP DATA، Mock، یا Hardcoded دارند را لیست کن.
برای هرکدام بگو: در کدام فایل است، چه داده‌ای شبیه‌سازی می‌کند، و برای جایگزینی با پیاده‌سازی واقعی چه چیزی لازم است.
```

## قبل از مهاجرت به دیتابیس واقعی (Migration)

```
می‌خواهم از [LocalStorage/Mock] به [نام دیتابیس واقعی] مهاجرت کنم.
۱. لیست کامل Repositoryهایی که باید تغییر کنند را بده (نه کل پروژه، فقط لایه‌ی Repository طبق معماری سه‌لایه).
۲. برای هرکدام، ساختار جدول/Schema پیشنهادی را بده.
۳. اگر جایی خارج از لایه‌ی Repository مستقیم به LocalStorage وصل است، آن را به‌عنوان مشکل معماری علامت بزن، چون نباید این‌طور باشد.
```

## بررسی چرخه‌ی Prompt Regression

```
در دو اصلاح اخیر، رفع یک باگ باعث بروز باگ جدید در بخش دیگر شده.
به‌جای اصلاح مستقیم این باگ تازه، اول Data Flow و معماری کامل بخش مرتبط را نشان بده
تا مشخص شود ریشه‌ی مشکل کجاست، نه فقط علامت آن.
```

## بررسی امنیتی سریع

```
این موارد را بررسی و گزارش کن:
۱. آیا هیچ Secret/کلید API در کد Frontend وجود دارد؟
۲. آیا همه‌ی Route/API های حساس، بررسی احراز هویت و نقش (Role) دارند؟
۳. اگر یک کاربر غیرمجاز مستقیم به URL صفحه Admin برود، چه اتفاقی می‌افتد؟
```

## پایان Sprint (اتصال به Checklist)

```
چک‌لیست فایل 05-CHECKLIST.md را روی وضعیت فعلی پروژه اجرا کن و برای هر بخش (الف تا و)
بگو کدام موارد رد و کدام قبول شده‌اند، با ذکر فایل/بخش مشکل‌دار.
```

```

</FILE>

---

<FILE path="VibeCoding-STD/README.md" tokens="475" lines="39">

```md
# STD — Vibe Coding Standard (V1)

این پوشه استاندارد شخصی من برای ساخت محصول با روش Vibe Coding است.
هدف: جلوگیری از تصمیم‌های معماری پنهانی که AI بدون اطلاع من می‌گیرد، و
جلوگیری از انباشت بدهی فنی که هنگام مهاجرت MVP به نسخه واقعی گریبان‌گیر پروژه می‌شود.

## این پوشه چیست و چه چیزی نیست

**هست:**
- یک مجموعه قانون کوتاه و عملی که قبل از شروع هر پروژه/Sprint به AI داده می‌شود.
- چک‌لیستی که خودم هر بار اجرا می‌کنم، نه سندی که فقط یک‌بار خوانده و فراموش شود.

**نیست:**
- یک کتاب معماری نرم‌افزار.
- یک متدولوژی کامل مدیریت محصول (Product OS کامل بماند برای نسخه‌های بعدی، اگر واقعاً لازم شد).
- وابسته به یک زبان یا فریم‌ورک خاص.

## ترتیب استفاده

1. **شروع هر پروژه جدید** → `01-CONSTITUTION.md` را به AI بده. این قوانین در تمام فازها ثابت‌اند.
2. **تشخیص فاز فعلی پروژه** → `02-PHASES.md` را چک کن تا بدانی الان کجای مسیر هستی و چه چیزی مجاز/ممنوع است.
3. **قبل از نوشتن هر Feature تازه** → اول `03-REUSE-FIRST.md` را چک کن؛ شاید نیازی به کد جدید نباشد.
4. **حین کدنویسی، هر وقت شک کردی** → `04-ANTIPATTERNS.md` را مرور کن تا ببینی الگوی خطرناکی تکرار نشده.
5. **پایان هر Sprint / قبل از رفتن به فاز بعد** → `05-CHECKLIST.md` را کامل اجرا کن.
6. **برای گفت‌وگو با Claude/ChatGPT** → از `06-PROMPTS.md` پرامپت آماده بردار، خودت از صفر ننویس.

## قانون طلایی این پوشه

> اگر جایی از پروژه با این استاندارد مغایرت داشت، مشکل از پروژه است، نه از استاندارد.
> اما اگر استاندارد در عمل دست‌وپاگیر یا غیرواقعی بود، خودِ استاندارد را اصلاح کن — این سند زنده است.

## نسخه‌بندی

- **V1 (فعلی):** حداقلی، عملی، قابل استفاده از همین پروژه اول. همین ۷ فایل.
- **V2 (بعداً):** بعد از ساخت ۳ تا ۵ محصول واقعی با این استاندارد، بخش‌های Foundation Library و Prompts و Examples گسترش پیدا می‌کنند.
- **V3 (بعداً):** بعد از استفاده‌ی واقعی و اصلاح مکرر، در صورت نیاز به Product Canvas / Blueprint کامل می‌رسیم.

هیچ‌وقت مستقیم از V1 به V3 نپر — تجربه واقعی هر پروژه باید نسخه بعدی را شکل بدهد، نه حدس و تئوری.

```

</FILE>
