# AI Job Hunter — Automated Job Discovery

An automated job discovery workflow built with n8n that finds remote job listings and sends matching opportunities to my email.

## Features
- Fetches remote jobs using the Remotive API.
- Splits job listings into individual items.
- Filters jobs using AI, machine learning, LLM, and AI automation keywords.
- Removes duplicate job URLs within the current execution.
- Sends job alerts through email.
- Runs on a daily schedule.

## Tech Stack
- n8n
- JavaScript
- Remotive REST API
- Gmail SMTP
- JSON

## Workflow
1. Schedule Trigger starts the workflow.
2. HTTP Request retrieves job listings.
3. Split Out separates the jobs.
4. JavaScript filters relevant opportunities.
5. Remove Duplicates removes repeated URLs within the current input.
6. Email node sends job alerts.

## Project Status
- Workflow published in n8n.
- Daily schedule configured.
- Email delivery tested successfully.

## Future Improvements
- Prevent previously emailed jobs from appearing in future runs.
- Add job location and experience-level filters.
- Improve email formatting and error handling.

## Purpose
This project demonstrates practical skills in workflow automation, API integration, JavaScript, and email notifications.
