---
title: Project Workflow & GitHub
layout: default
parent: DataSquad Handbook
nav_order: 3
---

# Project Workflow & GitHub

This page covers the end-to-end consultation workflow, from intake to completion, and how we use GitHub Projects, Google Drive, and Slack to stay organized.

| Purpose | Tool | Details |
| :--- | :--- | :--- |
| **Project Tracking** | **GitHub Projects** | Used for all project and professional development tracking. |
| **Documentation** | **Google Drive** | Used for work logs, specific resources, and longer descriptions. |
| **Communication** | **Slack** | Used for all internal, quick communication. |
| **Code Repository** | **GitHub** | Used for storing code and archives. |

**Quick links:**
[Project Intake Form](https://github.com/ucla-data-science-center/DataSquad/issues/new?template=project_intake.yml) · [Consulting Notes Template](https://docs.google.com/document/d/1b2DiDwqElha49yuCgEoS2PcNiIaDEnUFatNaXgOjrJA/edit?usp=sharing) · [Project Board](https://github.com/orgs/ucla-data-science-center/projects/3) · [Consulting Process Guidebook](https://docs.google.com/document/d/1LoTE03nb4yEA4wIidlxkrUsR8WP5TxkyG0KxP8c3K7c/edit?usp=sharing) · [Consultation Sign-in (in-person)](https://docs.google.com/spreadsheets/d/1X7zYSV_hMGimUJjCIFt7s03uweBVF9NmhoQlQhVRcrQ/edit?usp=sharing) · [Post-Consultation Survey](https://docs.google.com/forms/d/1Bb3VZMCscXhMQpehGnSUIRoDLrWmXKf2joTqxlueqa4/edit)

---

## Before the Meeting

1. **For in-person appointments:** Ask your patron to sign in using the [Consultation Sign-in Form](https://docs.google.com/spreadsheets/d/1X7zYSV_hMGimUJjCIFt7s03uweBVF9NmhoQlQhVRcrQ/edit?usp=sharing).
2. Create a [Project Intake Issue](https://github.com/ucla-data-science-center/DataSquad/issues/new?template=project_intake.yml) on GitHub. This automatically adds the project to the [GitHub Projects Dashboard](https://github.com/orgs/ucla-data-science-center/projects/3).
3. Add yourself and any other DSC members working on the project as **assignees**.
4. Set the linked Project to **DataSquad Projects** with the initial status **"New/Triage"**.

For in-person and walk-in appointments, also refer to the [Consulting Process Guidebook](https://docs.google.com/document/d/1LoTE03nb4yEA4wIidlxkrUsR8WP5TxkyG0KxP8c3K7c/edit?usp=sharing).

---

## During the Meeting

1. Create a new notes document in the **solo-projects-and-consultations** directory on Google Drive:
   - Make a copy of the [dsc-consulting-notes-template](https://docs.google.com/document/d/1b2DiDwqElha49yuCgEoS2PcNiIaDEnUFatNaXgOjrJA/edit?usp=sharing).
   - Name it: `notes_YYYY-MM_PatronFirstName-PatronLastName_Topic`
   - Example: `notes_2021-10_norman-powell_ucla-tree-maps`
2. Take **detailed notes** during the consultation.
3. If the consultation requires follow-up or recurring meetings, reuse the same notes document. Add notes for each new meeting on a **new tab**.

---

## After the Meeting

1. Move the Project Intake Issue to **"In Progress"** on the GitHub Projects Dashboard.
2. If you produced code or files for the patron, create a folder in the **solo-projects-and-consultations** directory:
   - Name the folder: `YYYY-MM_PatronFirstName-PatronLastName_Topic`
   - Example: `2021-10_norman-powell_ucla-tree-maps`
   - Move your notes document into the folder.
   - Add any code or deliverables to the folder.
3. **Communication:** Respond to Slack messages within **24 hours** or your next work shift.
4. **Seeking Help:** If you are stuck, seek support immediately by mentioning a peer or supervisor on the GitHub Issue (`@username`).

---

## Completing a Consultation

1. **For in-person appointments:** Link the notes document and folder (if applicable) in the [Consultation Sign-in Form (Responses)](https://docs.google.com/spreadsheets/d/1X7zYSV_hMGimUJjCIFt7s03uweBVF9NmhoQlQhVRcrQ/edit?usp=sharing) spreadsheet.
2. Email your patron using the template below.
3. Move the Project Intake Issue to **"Done"** on the GitHub Projects Dashboard.

### Follow-Up Email Template

> **Subject:** [DataSquad Consultation] Meeting Summary and Material
>
> Dear [Client Name],
>
> Thank you for scheduling an appointment with the DataSquad. It was a pleasure meeting you and learning more about your research.
>
> [Summarize everything you did during the meeting and how the client can proceed with that information]. I have also attached our meeting notes below for your reference [link the Google doc here].
>
> As you progress with your project, please feel free to schedule another consultation with me. We're happy to help and hope to serve as a resource for your data needs!
>
> Finally, we'd appreciate your feedback on today's session. Please take a moment to complete our brief [post-consultation survey](https://docs.google.com/forms/d/1Bb3VZMCscXhMQpehGnSUIRoDLrWmXKf2joTqxlueqa4/edit). Your input helps us improve and better support future consultations!
>
> Sincerely,
> [Your Name]

---

## GitHub Projects

[GitHub Projects](https://github.com/orgs/ucla-data-science-center/projects/3) is our source of record for tracking all consultations and projects.

- **Assign yourself** to an Issue using the **Assignees** option.
- **Update status** by moving issues through the columns: **New/Triage** → **In Progress** → **Done**.
- **Track progress** by ticking off checklist items within the Issue body.
