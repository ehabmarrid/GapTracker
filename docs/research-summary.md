# GapTracker Research Summary

## Problem Statement

Students often accumulate academic knowledge gaps without noticing them early enough. These gaps usually become visible during exercises, assignments, or exam preparation, when the time available to repair them is already limited.

GapTracker addresses the lack of a dedicated tool for managing understanding status. Existing productivity tools help students manage tasks, notes, or memorization, but they do not directly help students capture, prioritize, and close unclear academic topics.

## Research Context

- Participants: 36 undergraduate students.
- Research format: online survey and qualitative interviews.
- Target group: students managing several academic courses.
- Research period: not documented in the current repository materials.
- Recruitment method: not documented in the current repository materials.

The missing period and recruitment details should be added from the original course records before final publication.

## Research Method

The research included:

- A student survey with 36 respondents.
- User personas based on different learning contexts.
- User interviews focused on learning behavior, stress, uncertainty, and current tools.
- Competitive analysis of Notion, Todoist, Monday, Anki, and notes.
- Prototype decisions mapped to UX principles such as visibility of system status, recognition over recall, cognitive load reduction, error prevention, and psychological safety.

## Main Findings

Students struggle with detection, definition, and follow-through.

- Many students identify gaps during practice or close to exams, instead of during the class moment.
- Approximately 64% reported difficulty defining exactly what they did not understand.
- Approximately 53% postpone treatment of gaps even after identifying them.
- Students prefer simple, low-maintenance tools.
- Students avoid exposing lack of understanding because of social judgment, which supports a private and personal product direction.

The current repository materials provide percentages but not the raw survey export. Exact response counts should be verified from the original survey before replacing percentages with counts.

## Personas

### Dana: The First-Year Student

Dana is a first-year engineering student who wants confidence and structure. She worries about missing important topics and needs a simple way to record unclear points during class without interrupting her attention.

Primary need: reassurance and organized follow-up.

### Omar: The Working Student

Omar is a third-year student who works while studying. He has limited time and needs to know which gaps are most critical before an exam.

Primary need: prioritization and focused study.

### Ronit: The Teaching Assistant

Ronit wants to understand where students struggle across the class. In a future version, aggregated anonymous insight could help her adapt teaching and practice sessions.

Primary need: visibility into common learning difficulties.

## From Research To Product Decisions

| Research finding | Product decision |
|---|---|
| Students struggle to define unclear topics | Support quick gap capture with short descriptions and optional evidence |
| Students postpone treatment after noticing gaps | Show visible gap statuses and treatment actions |
| All gaps begin to feel equally urgent | Add criticality and priority indicators |
| Students notice gaps close to exams | Encourage in-the-moment capture during lectures and practice |
| Students prefer lightweight tools | Keep creation flows short and setup minimal |
| Students fear social judgment | Keep tracking private by default |
| Students need course structure | Support syllabus upload and course-topic extraction |

## Product Model

GapTracker converts a vague feeling into a managed learning object.

```text
Moment of confusion
  -> quick capture
  -> course/topic context
  -> priority level
  -> treatment action
  -> readiness update
```

The core object is the "gap": a specific unclear topic, attached to context and tracked until resolved.

## Interaction Model

The main flow is intentionally short:

1. Student notices confusion.
2. Student taps "New Gap".
3. Student records a short description or adds supporting evidence.
4. Student assigns the gap to a course or topic.
5. The system adds it to the dashboard.
6. Before an exam, critical gaps are surfaced first.
7. Student marks the gap as completed.
8. Readiness score updates.

## Design Principles

- Visibility of system status: the dashboard shows readiness and open gaps.
- Recognition over recall: students can capture a gap in the moment instead of reconstructing it later.
- Reduce cognitive load: the interface avoids heavy organization work.
- Error prevention: critical gaps are highlighted before exams.
- Privacy and psychological safety: the tool is personal and does not require public exposure.

## Competitive Positioning

GapTracker sits between notes, task managers, and memorization tools.

Unlike notes, it adds structure and status.
Unlike task managers, it keeps the academic understanding context.
Unlike flashcards, it supports unclear concepts and not only memorized facts.
Unlike Notion, it minimizes setup and maintenance.

## AI-Assisted Syllabus Concept

The syllabus-upload feature extends the product by letting students upload a course document. The system extracts course topics, creates a structured checklist, and lets students mark topics as completed. This connects course planning, gap tracking, and exam readiness in one workflow.

AI-generated topics should be treated as editable suggestions rather than unquestionable source of truth.

## Research Limitations

- The study used a relatively small sample of 36 respondents.
- Participants were mainly students from similar academic environments.
- Findings may not represent students from every institution or discipline.
- The current prototype requires further usability testing and long-term validation.
- The readiness model has not been validated as a predictor of academic performance.
- Exact raw survey counts are not included in the current repository materials.

## Future Direction

- Add editable review for AI-extracted syllabus topics.
- Improve manual course creation so it does not create generic placeholder topics.
- Test the dashboard and readiness model with students over a longer study period.
- Explore optional aggregated insights for teaching teams while preserving student privacy.
