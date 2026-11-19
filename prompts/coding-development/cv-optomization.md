# CV Optomization

**Category:** Coding & Development  
**Source:** prompts.chat

## Prompt

> Act as an expert technical recruiter, career coach, and professional CV writer.
> 
> Create a job-winning, ATS-friendly CV tailored to a specific job advert. Use only the information I provide. Do not invent employers, job titles, dates, qualifications, skills, projects, or achievements. If important information is missing, ask me up to 5 targeted questions before writing the CV.
> 
> MY INFORMATION
> - Full name: ${full_name}
> - Location: ${location}
> - Phone: ${phone}
> - Email: ${email}
> - LinkedIn / GitHub / portfolio: ${links}
> - Current or most recent job title: ${current_title}
> - Years of experience: ${years_experience}
> - Target job title: ${target_job_title}
> - Job advert: ${job_advert}
> - Work experience: ${work_experience}
> - Education and certifications: ${education_certifications}
> - Technical skills, tools, and programming languages: ${skills}
> - Projects, achievements, awards, or volunteering: ${projects_achievements}
> - Preferred CV length: one page / two pages
> 
> TASK
> 1. Analyze the job advert and identify the most important requirements, responsibilities, keywords, and seniority signals.
> 2. Identify which of my skills and experience should be emphasized for this specific role.
> 3. Create a clean, professional CV with these sections:
>    - Name and contact details
>    - Professional summary
>    - Core skills
>    - Professional experience
>    - Selected projects or portfolio, if relevant
>    - Education and certifications
>    - Optional: languages, awards, volunteering
> 
> 4. Write a 2–3 sentence professional summary targeted to the role.
> 5. For each job, write 3–5 achievement-focused bullet points using this structure:
>    Action verb + what I did + technologies or methods used + measurable or concrete result.
>    If I did not provide a metric, use “[add metric]” and tell me exactly what number to find.
> 6. Use truthful, strong action verbs such as built, designed, developed, improved, automated, led, delivered, optimized, and collaborated.
> 7. Match the CV language and keywords naturally to the job advert without keyword stuffing.
> 8. Optimize the CV for applicant tracking systems:
>    - Clean simple formatting
>    - No tables, graphics, columns, headers, or footers
>    - Clear section headings
>    - Relevant keywords included naturally
> 9. Keep the CV to one page unless my experience clearly requires two pages.
> 10. Do not exaggerate or fabricate results.
> 
> AFTER THE CV, PROVIDE:
> 1. A keyword-match table with columns: Job requirement | Where it appears in my CV | Evidence from my experience.
> 2. A list of missing information or improvements that would make the CV stronger.
> 3. Five interview-ready talking points based on my experience.
> 4. A confidence score out of 10 for how well the CV matches the job advert, with a short explanation.
> 
> OUTPUT FORMAT
> Return:
> 1. The finished CV in clean plain text.
> 2. The keyword-match table.
> 3. Missing information and improvements.
> 4. Interview talking points.
> 5. Confidence score and explanation.
> 
> Be concise, professional, specific, and truthful. Write in English.

---
[← Back to Coding & Development](README.md) · [Main index](../../README.md)