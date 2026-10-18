# PlanPilot Android Mobile Application Project Outline
### Prepared by Devon Moore
### Course: Mobile Application Development COM-437-OL01
### Instructor: Dr. Marwan Omar
### Date: October 18, 2026

Mobile Application Development — Project Concept and Design Specification

## 1. Project Description

**Purpose:** PlanPilot is an Android student productivity application designed to organize courses, assignments, and deadlines in one convenient location.

**Audience:** High-school and college students managing coursework across multiple classes.

**Platform:** Android smartphones; planned development in Android Studio using Kotlin and XML layouts.

**Goal:** Offer a straightforward dashboard for tracking upcoming work, priorities, and completion status.

## 2. Problem Addressing

**Challenge:** Students receive assignments and due dates through learning platforms, emails, syllabi, and classroom announcements. This scattered information makes it difficult to identify what needs attention first.

**Solution:** PlanPilot consolidates assignment details into a school-focused dashboard with due-date ordering, overdue indicators, priority labels, and reminders.

**Expected benefit:** Students can check one app instead of searching multiple sources, helping them plan study time and reduce missed deadlines.

## 3. Front/Back End Support

**Front end:** Kotlin-driven Android screens using XML layouts and familiar Material-style interface controls. Planned screens include Dashboard, Courses, Assignments, Add/Edit Assignment, and Assignment Details.

**Back end:** A local Room database is planned to persist courses and assignments on the device. Course records include course ID and name; assignment records include ID, course ID, title, due date, priority, notes, and completion status.

**Notifications and connectivity:** Android notifications are planned for deadline reminders. The core app is designed to work offline without requiring an account; cloud backup or sign-in would be a later enhancement.

## 4. Functionality

**Course management:** Add, edit, and delete courses.

**Assignment management:** Create, view, edit, and delete assignments with title, linked course, due date, priority, and optional notes.

**Tracking:** Sort by due date, identify overdue and upcoming tasks, and mark assignments complete.

**Validation and storage:** Require essential fields before saving and retain entries in local storage.

**Reminders:** Provide notifications ahead of assignment due dates, subject to implementation and testing.

## 5. Design (Wireframes)

**Design approach:** The app uses simple navigation, readable cards, clear due-date labels, and a prominent Add Assignment action. The following wireframes are conceptual rather than screenshots of a completed app.

### Wireframe A — Dashboard

```text

┌─────────────────────────────────┐

│ PLANPILOT       Today | Upcoming │

│ Due soon                         │

│ Database Quiz       Sep 3  HIGH │

│ Web Design Project  Sep 5   MED │

│ Android Outline     Sep 7   LOW │

│       + ADD ASSIGNMENT          │

│ Home       Courses     Tasks     │

└─────────────────────────────────┘

```

### Wireframe B — Add Assignment

```text

┌─────────────────────────────────┐

│ ADD ASSIGNMENT                  │

│ Title: _______________________  │

│ Course: [ Select course   ▼ ]   │

│ Due date: [ MM / DD / YYYY ]    │

│ Priority: Low | Medium | High   │

│ Notes: ______________________   │

│         SAVE ASSIGNMENT         │

└─────────────────────────────────┘

```

### Wireframe C — Assignment List

```text

┌─────────────────────────────────┐

│ ASSIGNMENTS     [Search...]     │

│ ☐ Database Quiz       Sep 3     │

│ ☐ Android Project     Sep 7     │

│ ☑ Chapter Questions   DONE      │

│ Filter ▼       Sort: Due date ▼ │

│ Home       Courses     Tasks     │

└─────────────────────────────────┘

```

### Wireframe D — Assignment Details

```text

┌─────────────────────────────────┐

│ ASSIGNMENT DETAILS              │

│ Android Project Outline         │

│ Mobile App Development          │

│ Due Sep 7     Priority: High    │

│ Finish outline and README       │

│       MARK COMPLETE             │

│          EDIT  | DELETE         │

└─────────────────────────────────┘

