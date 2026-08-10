# Task 2 – Business Analysis Requirements

**Team:** Team 40
**Feature:** Styled Login Page and Team Page
**Role:** Business Analyst
**Sprint:** Task 2 – Mock Sprint
**Date:** 10 August 2026

## 1. Purpose

The purpose of this feature is to provide users with a visually improved login experience and, following successful authentication, direct them to a Team Page that introduces Team 40 and its members.

The feature will use the existing Garage Boilerplate application and existing authentication functionality.

## 2. Scope

This sprint will deliver one complete feature consisting of:

* A visually styled version of the existing Login Page.
* A new Team Page for Team 40.
* A redirect from successful login to the Team Page.
* Team member information including each member's photo, name, role and short blurb.

The existing authentication system will be reused and should not be rebuilt as part of this sprint.

## 3. User Stories

### US-01 – Login Page

As a user, I want a clear and professionally styled Login Page so that I can easily understand how to sign in to the application.

### US-02 – Team Page

As an authenticated user, I want to be redirected to a Team Page after successfully signing in so that I can view information about Team 40 and its members.

## 4. Functional Requirements

### Login Page

**FR-01:** The existing Login Page must be visually styled according to the approved UX design.

**FR-02:** The existing email and password login functionality must remain available.

**FR-03:** The existing Google sign-in option must remain available.

**FR-04:** Styling changes must not remove or break existing login validation, error messages, loading states or authentication functionality.

**FR-05:** The email field, password field, sign-in button, Google sign-in button and account creation link must remain clearly identifiable and usable.

**FR-06:** Invalid login attempts must remain on the Login Page and display an appropriate error message.

### Login Redirect

**FR-07:** After successful authentication, the user must be redirected to the Team Page.

**FR-08:** The Team Page must use the route `/team`.

**FR-09:** Successful authentication through either email/password or Google sign-in must result in the same Team Page destination.

**FR-10:** An already authenticated user who accesses the sign-in page must be redirected to the Team Page rather than being required to sign in again.

### Team Page

**FR-11:** The Team Page must clearly display the team name, **Team 40**.

**FR-12:** The Team Page must contain a profile section or card for every member of Team 40.

**FR-13:** Each team member profile must contain:

* Member photo
* Member name
* Assigned project/sprint role
* Short personal or project-related blurb

**FR-14:** All team member information must be presented in a clear and consistent layout.

**FR-15:** The Team Page must follow the approved UX design.

## 5. Non-Functional Requirements

**NFR-01 – Responsive Design:**
The Login Page and Team Page must remain usable and readable on desktop and smaller/mobile screen sizes.

**NFR-02 – Accessibility:**
Text must be readable, interactive elements should have clear focus states, form fields should retain appropriate labels, and team member images should include appropriate alternative text.

**NFR-03 – Consistency:**
Fonts, spacing, colours, buttons, cards and other visual elements should follow a consistent design style.

**NFR-04 – Existing Functionality:**
Existing authentication functionality must not be broken by the new styling or Team Page feature.

**NFR-05 – Code Quality:**
Implementation must not introduce linting, type checking, build or existing test failures.

## 6. Acceptance Criteria

The completed feature will be accepted when:

1. The Login Page follows the approved UX design.
2. Email/password authentication continues to function.
3. Google authentication continues to function.
4. Existing login validation and error handling remain functional.
5. Successful login redirects the user to `/team`.
6. The Team Page clearly displays the name **Team 40**.
7. Every Team 40 member is represented on the Team Page.
8. Every member entry includes a photo, name, role and short blurb.
9. The Team Page matches the approved UX design.
10. The Login Page and Team Page are responsive and usable at different screen sizes.
11. Existing application functionality is not broken.
12. Relevant project quality checks complete successfully.

## 7. Out of Scope

The following items are outside the scope of this feature unless specifically requested by the Product Owner:

* Redesigning the sign-up page.
* Creating new authentication providers.
* Modifying Firebase authentication behaviour.
* Creating a database-driven team management system.
* Allowing users to add, edit or delete team members.
* Changing the Notes feature.
* Redesigning unrelated Dashboard functionality.
* Implementing administrative functionality.
* Allowing users to upload or edit team photographs through the application.

Team member information may be implemented as static content for the purposes of this Mock Sprint.

## 8. Constraints and Assumptions

* The existing Garage Boilerplate repository will be used.
* Existing authentication functionality should be reused rather than rebuilt.
* Team members will provide the correct photo, name, role and short blurb required for their Team Page profile.
* UX will create the visual design based on these requirements.
* Development must not begin until the UX design has been reviewed and validated by the BA.
* All work must follow the team's Git feature branch and Pull Request workflow.
* Task-specific deliverables must be stored in the Git repository and linked from Microsoft Planner.

## 9. Dependencies

* BA requirements must be completed before UX design begins.
* UX design must be completed and validated by the BA before development begins.
* Team members must provide their correct name, role, photo and blurb before the Team Page is finalised.
* Development depends on the existing authentication functionality in the Garage Boilerplate remaining operational.
* Each role must complete and hand off their assigned Planner task before the next task begins.

## 10. Requirements Traceability Summary

| User Story           | Related Requirements | Acceptance Criteria |
| -------------------- | -------------------- | ------------------- |
| US-01 – Login Page   | FR-01 to FR-06       | AC 1–4              |
| US-02 – Team Page    | FR-07 to FR-15       | AC 5–10             |
| Quality Requirements | NFR-01 to NFR-05     | AC 10–12            |

## 11. Handoff to UX

UX should create designs for:

1. The styled Login Page.
2. The Team Page layout.
3. Team member profile/card presentation.
4. Responsive behaviour for smaller screens.

The UX design should preserve all required login functionality and provide space for each team member's photo, name, role and short blurb.

Once the UX design is completed, it must be handed back to the BA for validation against the requirements before development begins.
