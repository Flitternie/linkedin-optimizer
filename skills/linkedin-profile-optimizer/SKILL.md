---
name: linkedin-profile-optimizer
description: Audit, rewrite, and—when explicitly authorized—edit LinkedIn profiles for CS PhD students and AI researchers seeking research-oriented industry roles. Use for profile positioning, recruiter readability, publication completeness, browser setup troubleshooting, and browser-assisted LinkedIn updates; do not use for job applications or social outreach.
---

# LinkedIn Profile Optimizer

Optimize the profile as a recruiter-facing research portfolio. Balance three goals:

1. A recruiter should understand the candidate's identity, level, domain, and strongest evidence within seconds.
2. Technical readers should find enough detail to judge the work.
3. Claims, dates, affiliations, and publication status must remain accurate.

## Define the requested outcome

- **Default workflow:** collect background, establish browser access, inspect the live profile, prepare changes, apply authorized edits, and verify the saved result in LinkedIn. A request to improve or update the profile authorizes ordinary edits within the requested sections, including help establishing the browser connection.
- **Explicit audit or draft request:** provide the requested review or replacement text. For an audit of the current profile, use the browser to inspect it when possible.

The default workflow is complete when the requested edits are saved and verified in the live browser. Prepare drafts while collecting information or repairing the connection. If authorization for edits is missing, prepare concrete changes before asking for it. Browser work can run in Codex or Claude Code without the ChatGPT desktop app.

Keep actions within the requested profile work. Messaging, job applications, public posts, following accounts, and unrelated settings require separate user direction.

Obtain explicit direction for deleting entries, replacing photos or banners, changing name or pronouns, contact details, location, or Open-to-Work visibility, unless those actions are already included in scope. Let the user authenticate directly in the browser.

## Collect missing source materials

Use the conversation, attachments, and user-identified files or links as the starting materials. Reuse available information and ask only for what the requested sections still need.

If background information is insufficient, proactively ask for a resume or CV as the easiest starting point. Accept a personal homepage, Google Scholar profile, publication list, portfolio, or pasted background instead; a resume is not mandatory, and the user need not provide every source. Ask in the user's language and bundle the initial request into one short message, for example:

```text
请发一份简历/CV，或提供个人主页、Google Scholar 等链接，也可以直接粘贴背景信息。也请提供目前的 LinkedIn 链接和目标岗位类型。如果有意向职位的 JD 或岗位链接，可以一并发来，方便针对性调整；这是可选项。已有的材料不用重复提供。
```

Optionally invite the user to share one or more target job descriptions or job links. Reuse any already supplied and proceed with the stated role family when none are available. If a job page cannot be retrieved, accept pasted JD text and continue with other available materials while waiting.

Read supplied public links with available retrieval tools. If a page is inaccessible, ask for an export, screenshot, or pasted relevant text. Use Google Scholar for publication facts and the candidate's other materials for employment history, graduation timing, and career goals.

If the user has no documents or prefers not to share them, collect the relevant facts directly: current role and affiliation, education and graduation timing, research focus, strongest projects or results, and target roles. Scale questions to the requested sections, accept redacted materials, and request contact details only when needed for the requested work.

Continue any review supported by existing material while awaiting answers. If the current LinkedIn profile is unavailable, prepare provisional text from verified background while actively establishing browser access; live inspection, editing, and verification remain pending. Ask focused follow-ups for consequential gaps or conflicting facts; omit unsupported claims from final profile text and leave unresolved fields out of live edits.

## Establish the source of truth

Review the current LinkedIn profile and the materials the user supplies, such as a CV, personal website, Google Scholar page, or publication list.

Build a private working inventory of:

- target role family and recruiting cycle;
- current title, affiliation, degree, and expected graduation date;
- research themes and searchable technical keywords;
- current and past appointments;
- two to four flagship projects;
- publications, venues, dates, URLs, and status;
- awards, skills, education, and contact links.

Use authoritative sources and reconcile conflicting records. Verify publication facts against official paper pages, DOI records, conference pages, or arXiv metadata. Ground dates, publication status, baselines, metrics, authorship, and organizational names in the available evidence.

Derive positioning from the candidate's own work and target roles.

When target JDs are available, identify the role's research themes, responsibilities, methods, systems skills, and expected level. Map those requirements to the candidate's documented experience, then tailor the headline, About, experience emphasis, featured projects, and skill ordering. Use recognizable JD terminology where the candidate's evidence supports it, and preserve official titles and factual claims. For multiple target roles, prioritize shared requirements and ask about priority only when their positioning differs materially. Discuss any gaps in experience with the user.

After the initial intake, ask focused follow-ups when a missing fact or choice affects accuracy or positioning, such as current affiliation, graduation timing, research versus engineering roles, the desired hiring year, or whether a sensitive item should be removed.

## Review in recruiter order

Evaluate the profile in this order:

1. Photo, banner, name, location, headline, and current organization
2. Open-to-Work preferences and contact paths
3. About
4. Featured
5. Experience
6. Education
7. Projects
8. Skills
9. Publications
10. Honors, certifications, languages, and older material

Prioritize the top card, first lines of About, current experience, and Featured section for recruiter readability.

## Apply the writing standard

Use concise, concrete English unless the user requests another language. Format LinkedIn About and experience fields with plain text, ordinary Unicode bullets, short paragraphs, and real blank lines for reliable rendering, accessibility, and search.

Lead with the contribution or outcome. A strong research bullet usually contains:

`Action + system or method + meaningful comparison + measured outcome`

Use a named baseline only when it makes the result easier to understand and the comparison is supported. Prefer “outperformed [baseline], improving [task metric] by [amount]” to vague phrases such as “achieved state-of-the-art performance.” Preserve qualifiers such as “up to,” “approximately,” “on benchmark X,” “preprint,” or “under review.”

Adapt the level of detail to each section:

- About: the memorable result and why it matters.
- Experience: ownership, method, and outcome.
- Project: the clearest technical explanation plus link.
- Publication: bibliographic identity plus one-sentence contribution.

## Optimize each section

Treat the lengths, counts, and structures below as starting points. Adapt them to the candidate's career stage, evidence, target JDs, and preferences.

### Headline

Aim for roughly 100–160 characters and three or four readable segments:

`Professional identity | Current affiliation | Core specialty | Strongest relevant credential`

Front-load role and affiliation. Emphasize degree and institution when relevant to the candidate's career stage. Keep the most valuable two or three technical themes; move secondary keywords to About, Experience, and Skills. Use official titles.

### About

Use visible paragraph breaks and keep the section easy to scan. A useful structure is:

1. One paragraph for identity, graduation timing, and research thesis.
2. One paragraph for current work and selected prior affiliations.
3. A “Selected work:” block with two to four bullets.
4. One short role-seeking statement when the user is recruiting.
5. One portfolio or publication link.

Roughly 900–1,400 characters often balances depth and readability for a research profile. Adjust the length to the user's preference and the amount of distinct evidence.

### Experience

Standardize research roles so they scan consistently:

```text
Research focus: [one concise theme].
• [Owned or developed X; method or scope; result.]
• [Second distinct contribution or validated outcome.]
• [Venue, deployment, or adoption signal when useful.]
• Hosts/Advisors: [names when they add useful context].
```

Use present tense for ongoing work and past tense for completed work. Two to four bullets are usually enough. Describe ongoing internships using information cleared for public sharing. Keep older roles shorter. Verify company, title, employment type, location, dates, and associated skills separately from the description.

### Featured

Feature three to five items that provide the shortest path to evidence:

- the strongest recent paper or launch post;
- one or two flagship projects;
- personal research homepage;
- Google Scholar or an equivalent publication index.

Prioritize recent, relevant work and verify that each link produces a usable preview.

### Education

Show the expected graduation date for an ongoing PhD when known. Use recognizable degree names and correct fields of study. Consolidate duplicate entries when they represent one degree, but retain genuine exchanges or second majors when completeness is useful and they do not crowd the main profile. Correct typos and inconsistent dates against the CV.

### Projects

Keep two to four flagship projects. Each should have:

- a descriptive name rather than only an acronym;
- a two- or three-sentence description of method and ownership;
- one or two comparison-based results;
- accurate dates, status, affiliation, and a stable paper, code, or project URL.

Use Projects to explain the strongest work in greater technical depth.

### Skills

Curate the visible top skills for recruiter search using the candidate's documented experience and target job descriptions. A useful ordering is:

1. primary research domain;
2. current specialization;
3. broad technical foundation;
4. core method or systems capability;
5. a complementary domain or implementation skill.

Include relevant tools and systems that demonstrate capability—often 12–25 skills total. Associate skills with relevant experiences when LinkedIn supports it. When proposing cleanup, consider the career value of existing skills and their endorsements; apply removals within the user's agreed scope.

### Publications

Create the union of the CV, homepage, and publication index, then deduplicate by normalized title, DOI, or arXiv identifier. For each item, verify:

- exact title;
- venue or truthful status such as “Preprint” or “Under review”;
- official or stable URL;
- publication date when an authoritative exact date is available;
- a one-sentence description of the contribution or result.

Accurate dates help recent work sort ahead of undated older papers. Enter dates at the precision supported by the source. If LinkedIn requires an unknown day, leave the field blank or ask the user.

LinkedIn may initially render only part of a long publication list. Scroll the actual page container until pagination completes, then verify the total number of distinct edit records and the presence of every expected title.

### Honors and secondary sections

Use a precise title, issuer, date, and one sentence explaining selectivity or the awarded work when that information is documented. Keep older debate, finance, test-score, language, or exchange information when it contributes breadth and remains below the primary research sections. Recommend removal only when it materially distracts from the target role.

### Open-to-Work and contact information

Align job-title preferences with the About section, generally using three to five standard titles. Confirm seniority, geography, remote-work preference, start date, and visibility with the user before changing those preferences.

Verify that a stable portfolio URL and a professional contact method are available. Treat phone number, birthday, email visibility, and precise location as privacy-sensitive.

## Prepare and use the browser

Read [references/browser-setup.md](references/browser-setup.md) when establishing browser access or troubleshooting navigation, fields, saving, or lazy-loaded lists. Start a read-only connection check alongside source collection.

Prefer available browser tools and verify access to the intended session. Actively diagnose and repair connection problems using the linked reference, including setup of a needed browser client or integration when permitted. Preserve unrelated settings and ask the user for actions requiring their participation, such as authentication, browser permissions, or a host restart.

If browser access remains blocked after meaningful diagnostics and a supported alternative, report the failure, attempted fixes, unfinished edits, and minimum user action needed to resume.

Once connected, inventory existing values, resolve the exact target, change one logical section at a time, disable routine network notifications unless requested, save, and verify the rendered result. Follow the authentication procedure in the browser reference.

Save original values and a short per-section progress record in `.linkedin-profile-work/` under the user's working directory, separate from the installed skill. Track each section as planned, saved, or verified. After an interruption, reread the live section before retrying; use snapshots to support restoration when requested. Record profile content and edit status only, keeping credentials and browser session secrets out of these files.

## Final quality check

Before handing off, verify:

- for the default workflow, each completed edit was saved and checked in the live browser, and any unfinished section is explicitly reported;
- the first screen identifies professional identity, current affiliation, and specialty, with education where relevant;
- the About section has real blank lines and readable bullets;
- current role, graduation date, target role, and Open-to-Work titles agree;
- flagship claims preserve baselines, datasets, qualifiers, and metrics;
- tense, punctuation, date formats, and role descriptions are consistent;
- the newest projects and publications appear before older work where dates permit;
- URLs open and no duplicate publications or experiences were introduced;
- long lists were fully paginated before counting;
- no post, message, application, privacy change, or notification was triggered unintentionally.

Report the material changes, verification results, unfinished work, and any remaining user decisions. Keep candidate-specific working materials separate from reusable skill files, templates, and examples.
