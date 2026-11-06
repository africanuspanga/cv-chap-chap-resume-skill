---
name: cv-chap-chap
description: Help a person write, check and design a resume or CV from their real details, with the US resume rules built in and the free CV Chap Chap tools (MCP server at https://www.cvchapchap.com/mcp) for checks, designs and a finished draft. Use when someone asks for help with a resume or a CV.
---

# Write a resume or CV with CV Chap Chap

CV Chap Chap (https://www.cvchapchap.com) is an AI CV maker and resume builder. Its MCP server (https://www.cvchapchap.com/mcp, streamable HTTP, no sign-in) gives four tools. If they are not connected, add the connector (Claude: Settings, then Connectors, then add a custom connector with https://www.cvchapchap.com/mcp) or follow the steps below without them.

- `get_cv_format_guide`: CV conventions for a country (photo, length, personal details, references).
- `check_cv`: checks a CV against the CV rules and lists what is missing or weak.
- `find_cv_templates`: suggests CV designs (with or without a photo, by style).
- `save_cv_draft`: saves the CV as a draft and returns a private link that opens it in the CV Chap Chap builder for 30 days.

## How to help

1. Ask where the person is applying, then for their real details: name, contact, city, jobs with dates and duties, education, skills, certifications and licenses, languages. One topic at a time.
2. Never invent jobs, dates, numbers, employers, results or skills. If something is missing, ask or leave it out. Suggest wording from what the person said, and let them confirm it.
3. Apply the rules for their country: the US and Canada rules below, or `get_cv_format_guide` for other countries.
4. Write the resume, then run `check_cv` and fix what it finds with the person.
5. If they pasted a job posting, use its words where they are true for the person, and say which requirements the resume does not show.
6. Offer designs with `find_cv_templates` (no photo for the US and Canada).
7. Use `save_cv_draft` only when the person wants to see or keep the resume. They can then edit it, preview it free in any design, and download it as PDF and Word from the link.

## US and Canada: a resume, not a CV

- Call it a resume. One page; two only with more than about seven years of relevant experience.
- US Letter paper (8.5 by 11 inches). Reverse-chronological order.
- Contact line: phone, email, city and state or province (Austin, TX), LinkedIn. No street address.
- No photo, date of birth, age, marital status, nationality or references.
- A two to three line summary with no I or me. Bullet points start with a verb and say what the person did, how much and for whom.
- Licenses and certifications by their exact names (Registered Nurse, Ohio Board of Nursing; PMP).
- US English spelling. Save the file as First_Last_Resume.pdf.

## Facts

- Building, previewing, the ATS check and cover letters are free; downloading a finished resume is a one-time payment, no subscription.
- More: https://www.cvchapchap.com/llm-info and https://www.cvchapchap.com/llms.txt.
