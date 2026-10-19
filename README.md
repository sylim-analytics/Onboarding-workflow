# Onboarding Command Center

A clickable prototype of a new-hire onboarding tracker, designed to replace scattered emails and spreadsheets with one place to manage every hire from intake to day 90.

**Live demo:** https://sylim-analytics.github.io/Onboarding-workflow/
**Status:** the production version is being built in Microsoft 365 (see below).
**Built with:** HTML, CSS, JavaScript, Claude AI, and Visual Studio Code.

> The demo is a design mockup. All names, emails, links, and data are fictional, and nothing is saved to any external system.

## The problem

Onboarding a new hire involves many people and many small tasks: workspace setup, IT and software requests, badges, training, announcements, and follow-ups. Tracking these by email and hand-built spreadsheets makes it easy to miss steps and hard to see where each hire stands.

## What it does

- **Dashboard:** live progress for every active hire, with status and percent complete, filtered by role (admin sees all hires, supervisors see only theirs).
- **Intake log:** records each new hire the moment the request arrives, including type and department.
- **Hire checklist:** a tailored task list per hire, split into pre- and post-onboarding and by owner (supervisor or admin), with ticket numbers, memos, and one-click links to the right request forms.
- **Smart task rules:** one master task list drives every checklist. Tasks apply by hire type (Employee, Intern, Internal Transfer, Contractor), and some become optional automatically for remote hires.
- **Form responses comparison:** hire-intake form answers laid out side by side for easy comparison.
- **Notification timeline:** a preview of four automated reminder emails (hire logged, 5 days before start, start day, 7 days after).
- **Pre-filled emails:** certain tasks open a ready-to-send email with the hire's details filled in.

## My role

While covering for two administrators, I saw that each ran onboarding differently and that the information they needed was scattered across emails, files, and systems. I defined the requirements and task rules for a single, consistent workflow, then built the prototype with Claude (Anthropic's AI assistant) and Visual Studio Code.

## Built with

HTML, CSS, and vanilla JavaScript in a single file, with no frameworks. Browser local storage keeps demo changes between visits.

## Production build (in progress)

I'm building the real version in Microsoft 365, using this prototype as the design reference.

**Done so far**
- SharePoint Lists are set up for the data (Hires, Master Tasks, Hire Tasks)
- Power Automate flows are connected to the lists. When a new hire is entered in the intake log, a flow creates their checklist automatically based on hire type (Employee, Intern, Internal Transfer, or Contractor).

**In progress**
- Reminder emails
- Power Apps screens for the dashboard and checklist
- Organizing each section (dashboard, intake log, checklists) into a clean layout on the SharePoint site

## Run it locally

Download `index.html` and open it in any browser.
