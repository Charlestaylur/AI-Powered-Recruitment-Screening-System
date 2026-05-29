# AI-Powered Recruitment Screening System

> Automated hiring workflow that scores resumes, updates a CRM, and triggers candidate communications so recruiting teams spend less time on admin and more time on decisions.

**Industry:** Recruitment Agencies, HR Departments, Staffing Firms

## Demo

[Watch the full walkthrough →](https://drive.google.com/file/d/13MaJ9Xzf0DWPbHu-xkXWPG9bcZA35nIi/view?usp=sharing)

---

## The Problem

Every time the agency posted a job, applications flooded in within hours. Their internal team spent the majority of each day downloading resumes, opening them one by one, and manually checking each candidate for fit against the job requirements. The screening backlog delayed hiring decisions and created inconsistency in how candidates were evaluated and communicated with.

---

## The Solution

I built an end-to-end recruitment automation system in n8n that handles the entire early-stage screening process. When a candidate applies via email or form, the system extracts their resume details, scores them against the active job description using an AI agent, logs the result to an Airtable CRM, and notifies the team. From the dashboard, the team moves candidates forward or triggers a rejection with a single click.

---

## How It Works

1. **Application intake** — The system monitors a Gmail inbox and a form endpoint for new candidate submissions. Both channels feed into the same workflow.
2. **Resume extraction** — The workflow parses the attached resume and pulls structured candidate data including name, contact details, experience, skills, and education.
3. **AI scoring** — An AI agent compares the extracted profile against the job description and produces a fit score with a short justification. This runs without any human input.
4. **CRM logging** — The candidate record, score, resume data, and AI notes are written to an Airtable base as a new row. The hiring team sees every applicant in one place, ranked and documented.
5. **Team notification** — A Slack message is sent to the hiring channel with a summary of the new candidate and their score, so the team is never in the dark.
6. **One-click decisions** — From Airtable, the recruiter clicks to advance or reject. The system detects the status change and sends the appropriate email automatically, either a next-step message or a polite rejection.

---

## Tech Stack

| Tool | Role |
|---|---|
| **n8n** | Core workflow orchestration and automation logic |
| **AI Agent (OpenAI)** | Resume parsing, candidate scoring, fit analysis |
| **Airtable** | Candidate CRM and hiring pipeline dashboard |
| **Gmail** | Application intake and outbound candidate communications |
| **Slack** | Internal team notifications on new candidates |

---

## Results

- Recruiting team reclaimed 20+ hours per week previously spent on manual resume review
- Candidate response time dropped from days to minutes as emails are now triggered automatically
- Every applicant is scored against the same criteria, removing inconsistency in early-stage screening
- The system handles volume spikes without any increase in admin workload

---

## About

Built by **Charles Emmanuel** — AI & Automation Systems Engineer.                                                                         
Lagos, Nigeria | [LinkedIn](https://linkedin.com/in/charles-emmanuel-automation) | charlestaylurr@gmail.com

I build systems that remove repetitive manual work so teams can focus on what actually matters. If your business is losing time or money to broken processes, reach out.
