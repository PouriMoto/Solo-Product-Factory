🚀 Product OS v1

A Framework for Vibe Coding & AI-Native Development

---

📑 Table of Contents

· Overview
· Philosophy
· Repository Structure
· Documentation Standards
· File Naming Convention
· Document Types
· Versioning Strategy
· Cross-Reference System
· Development Workflow
· Decision Log System
· Getting Started
· Contributing
· License
· Quick Reference

---

🎯 Overview

Product OS v1 is a comprehensive framework and knowledge base for building software products using Vibe Coding — a development approach optimized for collaboration with AI assistants like ChatGPT, Claude, and similar tools.

What This Repository Provides

Feature Benefit
📄 Standardized Documentation Works with any AI assistant
✅ Executable Checklists Step-by-step guides for each phase
🎯 Prompt Library Consistent AI interactions
📝 Decision Logs Prevents recurring discussions
📋 Playbooks Rapid product launches

What is Vibe Coding?

Vibe Coding is a methodology where you:

```
🧠 Think in Layers    →  Understand → Decide → Execute
📦 Work Atomic        →  One File = One Concept
🤖 AI as Pair Programmer → Clear prompts, consistent outputs
📈 Build Incrementally → Sprint-based with stable releases
📚 Document Everything → Every decision has a home
```

---

🧠 Philosophy

Core Principles

# Principle Description
1 Single Source of Truth Every concept has exactly one definitive file
2 Atomic Files Each file covers one topic only (700-1000 words max)
3 Action First Must answer: "After reading, what should I do?"
4 Build vs Buy Use existing solutions first, build only when necessary
5 AI Native Processes designed for AI execution with dedicated prompts
6 Vibe Coding Friendly No huge files, no academia, clear steps
7 Living Document A living system, not a static book

---

📁 Repository Structure

```
Product-OS/
│
├── Sprint-00/          # 🏗️ Foundation & Standards
│   ├── SPR-README-001-Repository-Overview.md
│   ├── SPR-ARCH-001-Repository-Architecture.md
│   ├── SPR-STD-001-Document-Standards.md
│   ├── SPR-STD-004-Authoring-Protocol.md
│   └── SPR-TOC-001-Repository-TOC.md
│
├── Sprint-01/          # 💡 Product Thinking & Canvas
│   ├── PRN-*-*.md      # Product Principles
│   ├── CAN-*-*.md      # Canvas Components
│   └── ...
│
├── Sprint-02/          # 📐 Blueprint & Design
│   ├── BP-DISC-*.md    # Discovery
│   ├── BP-DES-*.md     # Design
│   └── BP-ARCH-*.md    # Architecture
│
├── Sprint-03/          # 🔧 Foundation
│   ├── FD-AUTH-*.md    # Authentication
│   ├── FD-BILL-*.md    # Billing
│   └── FD-DB-*.md      # Database
│
├── Sprint-04/          # ⚙️ Development Workflow
│   ├── PRM-*-*.md      # Prompts
│   ├── TMP-*-*.md      # Templates
│   └── QA-*-*.md       # Quality Assurance
│
└── Sprint-05/          # 🚀 Execution & Playbooks
    ├── EX-*-*.md       # Example Projects
    └── PLY-*-*.md      # Playbooks
```

---

📝 Documentation Standards

File Header

Every file starts with this standard header:

```markdown
# Title of File

**File ID:** CAT-TOPIC-001
**Version:** 1.0
**Sprint:** Sprint-03
**Status:** Stable
**Last Update:** YYYY-MM-DD

---
```

File Structure

Most files follow this structure (sections may be omitted):

Section Purpose
Purpose What this file is about
Why Why this concept matters
When When to use this file
Inputs What you need before starting
Outputs What you'll have after completion
Checklist Step-by-step action items
Best Practices Recommended approaches
Common Mistakes What to avoid
Tools Recommended tools and services
Prompt AI prompt (only in PRM-* files)
Related Files Cross-references

The 3-Layer Structure

Every file follows the Understand → Decide → Execute pattern:

```
1️⃣ Understand  →  What is this concept?
2️⃣ Decide      →  What decision do I need to make?
3️⃣ Execute     →  What exactly should I do?
```

---

🏷️ File Naming Convention

Format

```
[Category]-[Topic]-[Number]-[Title].md
```

Categories

Code Category Usage
SPR Sprint Sprint-specific files (Sprint-00 only)
PRN Principle Core principles and philosophies
CAN Canvas Product Canvas components
BP Blueprint Product design and architecture
FD Foundation Technical foundations
PRM Prompt AI prompts and interactions
TMP Template Reusable templates
QA Quality Testing and quality standards
EX Example Case studies and examples
PLY Playbook Execution guides

Examples

```
FD-AUTH-001-Authentication-Overview.md
BP-ARCH-001-Architecture.md
PRM-BE-001-Backend-Prompt.md
CAN-PRB-001-Problem.md
```

Document ID

Each file has a unique Document ID (CAT-TOPIC-XXX) that remains constant even if the file moves between sprints.

---

📚 Document Types

Type Code Description
Knowledge PRN, CAN, BP, FD Teaches concepts, must include Action First
Decision SPR-STD-010, BP-GNG-* Documents important decisions
Checklist QA-*, -CHK- Step-by-step execution guides
Template TMP-* Reusable templates for various needs
Prompt PRM-* AI-specific prompts (never in Knowledge files)

---

🔢 Versioning Strategy

Status Levels

Status Meaning
Draft Initial version, in progress
Stable Complete and reviewed, ready for use
Reviewed Final version, approved and frozen

Version Numbers

· Format: MAJOR.MINOR (e.g., 1.0, 1.1, 2.0)
· Increment for significant changes
· Major versions indicate breaking changes

---

🔗 Cross-Reference System

How to Reference

```markdown
> For details on Authentication, refer to [FD-AUTH-001](Sprint-03/FD-AUTH-001-Authentication-Overview.md).
```

Related Files Section

Every file ends with:

```markdown
## Related Files

- [FD-AUTH-001](Sprint-03/FD-AUTH-001-Authentication-Overview.md)
- [FD-AUTH-002](Sprint-03/FD-AUTH-002-Authentication-Providers.md)
```

Key Rules

Rule Description
🚫 No Duplicate Content Reference instead of repeating
🔗 Always Link Include document ID and path
📌 Keep Relationships Maintain related files sections

---

🔄 Development Workflow

Sprint Structure

Each Sprint has: Goal → Outputs → Result

Sprint Breakdown

Sprint Focus Key Outputs
00 Foundation & Standards Repository structure, protocols, TOC
01 Product Thinking Principles, Canvas, Problem definition
02 Blueprint & Design Discovery, Validation, Architecture
03 Foundation Starter Kit, Auth, Database, Billing
04 Development Workflow Prompts, Templates, QA, Git Workflow
05 Execution Example projects, Playbooks

⚠️ Critical Rule

Once a Sprint is complete, it is FROZEN. No changes allowed.

New ideas go to:

· 📝 Decision Log (if important for current version)
· 🚀 Product OS v2 (if requires breaking changes)

---

📝 Decision Log System

🎯 Purpose

A lightweight system to capture decisions and ideas without breaking momentum. Every thought goes to the Decision Log, not into active development.

How It Works

Step Action
1 Log First — Any idea → Create decision file
2 Don't Act — Never implement during current sprint
3 Review Later — Evaluate during sprint planning
4 Keep Simple — Max 200 words per decision

File Structure

```markdown
# Decision: [Title]

**Decision ID:** SPR-DEC-001
**Date:** YYYY-MM-DD
**Status:** Proposed | Approved | Rejected | Postponed
**Related Files:** [FD-AUTH-001]

---
## Context
What triggered this decision?

## Options Considered
1. Option A - Pros/Cons
2. Option B - Pros/Cons

## Decision
What we chose and why.

## Impact
What changes because of this.

## Action
- [ ] What to do now
- [ ] What to defer

## For Future
How this affects v2 or later sprints.
```

Decision Lifecycle

```
💡 Idea → 📝 Log it → 🔍 Review → ✅ Approve → 🚀 Implement
                                ↓
                            ❌ Reject
                                ↓
                            ⏸️ Postpone (v2)
```

Status Tracker

Status Meaning Next Action
Proposed New idea, needs review Review in next sprint planning
Approved Ready for implementation Add to next sprint backlog
Rejected Won't implement Document why, close
Postponed Good idea, but for v2 Move to v2 backlog

Quick Command

Simply write:

```
"Log: Should we use Firebase instead of Supabase for auth?"
```

The system creates:

```
Sprint-00/Decisions/SPR-DEC-XXX-Firebase-vs-Supabase.md
```

Benefits

Benefit Description
⏭️ No Interruption Keep writing, just log it
📂 No Duplication All decisions in one place
🧠 No Forgetting Every idea is captured
😌 No Regret Review decisions properly later
🎯 No Scope Creep Current sprint stays focused

---

🚀 Getting Started

Using This Repository

1. Start with Sprint 00 — Read the standards and protocols
2. Follow the sprint order — Each sprint builds on previous ones
3. Use file IDs — Request files by ID (e.g., "FD-AUTH-001")
4. Stay atomic — One file = one concept
5. Keep it alive — Update based on real project experience

Working with AI Assistants

Simply request a file by its ID:

```
"Show me FD-AUTH-001"
"Update BP-ARCH-001 to version 1.1"
"Create a new file FD-NEW-001 with [description]"
```

The AI will respond with exactly that file's content, following all standards.

Creating New Files

Step Action
1 Choose the right category (PRN/CAN/BP/FD/PRM/TMP/QA/EX/PLY)
2 Select a topic code
3 Assign the next available number
4 Use the standard file structure
5 Add cross-references
6 Set status to "Draft"
7 Include in the TOC

Avoiding Scope Creep

· ❌ Don't change completed sprints
· 📝 Log new ideas in Decision Log
· 🚀 Save breaking changes for v2
· 🎯 Keep each sprint focused

---

🤝 Contributing

Guidelines

# Guideline
1 Follow all documentation standards
2 Maintain atomic files (one topic = one file)
3 Keep content actionable (Understand → Decide → Execute)
4 Add cross-references, not duplicate content
5 Update version and status when modifying
6 Never change frozen sprints

Pull Request Process

1. Review existing content to avoid duplication
2. Ensure your file follows all standards
3. Add related files section
4. Update the repository TOC
5. Request review from maintainers

---

📄 License

Product OS v1 is licensed under the MIT License.

✅ Allowed ❌ Restrictions
Commercial use None (with copyright notice)
Modification 
Distribution 
Use in own products 

---

🔗 Quick Reference

Most Important Files to Read First

# File Description
1 SPR-STD-004 Authoring Protocol (The Constitution)
2 SPR-TOC-001 Complete Table of Contents
3 PRN-PRD-001 Product Thinking Principles
4 BP-ARCH-001 Architecture Overview
5 FD-START-001 Starter Kit Foundation
6 PRM-SYS-001 System Prompt Template
7 PLY-PRD-001 New Product Playbook

Common File Requests

Request File
New product planning CAN-OVR-001
Customer definition CAN-CUS-001
MVP scope CAN-MVP-001
Architecture design BP-ARCH-001
Authentication setup FD-AUTH-001
Database selection FD-DB-002
Billing integration FD-BILL-001
System prompt PRM-SYS-001
PRD template TMP-PRD-001

---

📊 Repository Status

Version Status Last Updated
v1.0 ✅ Stable 2026-01-09

---

🙏 Acknowledgments

This framework was developed through collaboration between human product thinkers and AI assistants, proving that Vibe Coding is not just possible but powerful.

---

"Product OS is not a book. It's a living system. Every real product built improves it."

---

Built with ❤️ for Vibe Coders everywhere
