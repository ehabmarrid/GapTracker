# GapTracker

GapTracker is a research-driven academic knowledge-gap management web app that helps students capture unclear topics, organize course material, and monitor exam readiness.

The project combines UI/UX research with a working public prototype. It focuses on a student problem that is easy to recognize: knowledge gaps are often noticed too late, poorly defined, and left untreated until exam pressure builds.

## Live Demo

**[Open GapTracker](https://gaptracker-academic-knowledge-gap-management-117567148344.europe-west2.run.app/)**

The deployed prototype runs on Google Cloud Run and is intended for portfolio and academic review.

<p align="center">
  <a href="docs/images/dashboard.png">
    <img
      src="docs/images/dashboard.png"
      alt="GapTracker dashboard"
      width="700"
    >
  </a>
</p>

## Product Preview

<table>
  <tr>
    <th>Dashboard</th>
    <th>Course Directory</th>
    <th>Course Detail</th>
  </tr>
  <tr>
    <td valign="top">
      <img src="docs/images/dashboard.png" alt="GapTracker dashboard" width="200">
    </td>
    <td valign="top">
      <img src="docs/images/courses-directory.png" alt="GapTracker course directory" width="385">
    </td>
    <td valign="top">
      <img src="docs/images/course-detail.png" alt="GapTracker course detail" width="200">
    </td>
  </tr>
</table>

## What GapTracker Does

- Creates a personal academic workspace after sign-in.
- Starts new users with an empty dashboard instead of predefined demo courses.
- Lets students add courses manually.
- Supports syllabus upload for AI-assisted course-topic extraction.
- Tracks syllabus progress and course readiness.
- Helps students record and prioritize understanding gaps.
- Highlights critical gaps that need attention before exams.

## Problem

Students often accumulate hidden academic knowledge gaps during lectures, practice, and assignments. By the time those gaps become obvious, the student may already be close to an exam and under pressure.

The research behind GapTracker identified three recurring issues:

- Students often notice gaps too late.
- Students struggle to define exactly what they did not understand.
- Students postpone treatment of gaps even after noticing them.

## Solution Model

GapTracker turns a vague moment of confusion into a trackable learning object:

```text
Moment of confusion
  -> quick capture
  -> course/topic context
  -> priority level
  -> treatment action
  -> readiness update
```

This gives students a clearer answer to three questions:

- What do I still not understand?
- What matters most before the exam?
- What have I already resolved?

## AI-Assisted Syllabus Processing

The syllabus feature is designed to accept an uploaded course document and use an AI model to:

1. Identify course structure.
2. Extract topics and learning units.
3. Convert the extracted content into a trackable checklist.
4. Connect completed topics with the readiness dashboard.

### AI and Free-Tier Constraints

The deployed prototype uses Gemini API features with free-tier constraints. AI actions may be temporarily unavailable if quota or rate limits are reached.

AI-generated syllabus topics should also be reviewed by the student. Extracted topics may require correction depending on the quality and structure of the uploaded document.

## Research Foundation

GapTracker was designed through a structured UI/UX research process focused on how university students identify, describe, prioritize, and resolve academic knowledge gaps.

The initial academic research phase was completed collaboratively by **Ehab Marrid and Saleem Trudi** and included:

- A student survey with 36 respondents
- Three qualitative user interviews
- User personas representing different learning contexts
- Competitive analysis of existing productivity and study tools
- Mapping research findings to product and interaction decisions
- UX principles including visibility of system status, recognition over recall, cognitive-load reduction, error prevention, privacy, and psychological safety

The research showed that students often notice knowledge gaps too late, struggle to define exactly what they did not understand, and postpone addressing gaps even after identifying them.

### Research Documents

- [Full HCI User Research Report](docs/hci-user-research-report.md)
- [Research Summary](docs/research-summary.md)
- [Research Models Presentation](docs/GapTracker-Research-Models.pptx)

## Research-To-Design Decisions

| Research finding | Product decision |
|---|---|
| Students struggle to define unclear topics | Support quick gap capture with short descriptions and optional evidence |
| Students postpone treatment | Show visible statuses and treatment actions |
| All gaps can feel equally urgent | Add criticality and priority indicators |
| Students notice gaps close to exams | Encourage in-the-moment capture during study |
| Students prefer lightweight tools | Keep setup and creation flows short |
| Students fear social judgment | Keep tracking private by default |

## Technology

### Application and AI

- Google AI Studio
- Gemini API
- Responsive web application

### Deployment

- Google Cloud Run

### Design and Research

- Figma
- UI/UX research
- User surveys and interviews
- Competitive analysis

## Repository Scope

This repository presents the deployed GapTracker prototype together with its UI/UX research, product documentation, screenshots, and design materials.

The application is publicly available through the live demo. The application source code is not currently distributed through this repository.

## Repository Contents

```text
GapTracker/
  README.md
  .gitignore
  docs/
    hci-user-research-report.md
    research-summary.md
    GapTracker-Research-Models.pptx
    images/
      dashboard.png
      courses-directory.png
      course-detail.png
```

## Prototype Status and Limitations

- GapTracker is a functional portfolio and academic prototype.
- Gemini-powered features may be temporarily unavailable when public API quotas or rate limits are reached.
- AI-extracted syllabus topics should be reviewed and corrected by the student before being treated as final.
- The readiness score is a product-support indicator and has not been scientifically validated as a predictor of exam performance.

## My Contributions

- Continued the project independently after the initial research phase.
- Redesigned and expanded the original product concept.
- Developed the functional GapTracker web application.
- Implemented AI-assisted syllabus extraction and topic generation.
- Designed the current user interface and product workflows.
- Added course, gap, readiness, and syllabus-management functionality.
- Deployed the application to Google Cloud Run.
- Prepared the GitHub README, research documentation, and project attribution materials.

## Usage and Rights

This repository is publicly available for portfolio and academic-review purposes only.

The current GapTracker application, later product development, deployment, interface design, and technical documentation were created independently by **Ehab Marrid**.

The original academic research phase was completed collaboratively by **Ehab Marrid and Saleem Trudi** and remains credited to both contributors.

Copyright © 2026 Ehab Marrid for the independently created application and documentation. All rights reserved. No permission is granted to reproduce, modify, distribute, sublicense, or commercially use the independently created application materials or repository contents without prior written permission.

Rights and attribution for the jointly created research materials remain with their respective contributors.
