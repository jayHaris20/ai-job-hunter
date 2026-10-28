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
## How It Works

1. Schedule Trigger starts the workflow automatically according to the configured daily schedule.
2. Edit Fields (Details) Sets sample job details such as job title, company name, and application link. These are currently configured as static values.
3. HTTP Request fetches remote job listings from the Remotive API.
4. Split Out separates the jobs array into individual job items.
5. Code in JavaScript filters job listings using relevant AI, machine learning, LLM, and automation-related keywords.
6. Remove Duplicates removes repeated job URLs within the current execution.
7. Edit Fields (Job Alert) formats job information into a readable job alert containing the position, company, category, and application link.
8. Send an Email sends the matching job details to the configured email address using Gmail SMTP.
<img width="593" height="299" alt="image" src="https://github.com/user-attachments/assets/899f071e-e00b-4945-9c22-71fe28251753" />


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
