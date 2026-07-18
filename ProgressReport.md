# Progress Report, Week 2

**Author:** Yashal Manaiem Javaid
**Programme:** BS Psychology, COMSATS University Islamabad
**Group:** 43
**Project:** SafeX Solutions, Mental Health Awareness Research
**Reporting period:** Week 2
**Status:** Completed

---

## Objective for the week

Design, build, and document the Mental Health Awareness Research component of Group 43's SafeX research project as my individual Week 2 contribution, continuing the group's Week 1 work and integrating cleanly with the other members' modules.

## Work completed

**Research design.** Reviewed the Week 1 group scope and defined the specific angle of my module: measuring the awareness gap rather than duplicating the broader mental health overview being handled elsewhere in the group. Framed three research questions around awareness, stigma, and barriers.

**Survey instrument.** Designed a sixteen-item questionnaire across three sections: demographics, awareness and attitudes (including four Likert-scale items and one self-rating scale), and barriers, preferences, and open feedback. Reviewed all items for neutrality of wording. Kept the instrument short (around five to seven minutes) to protect the response rate.

**Deployment.** Built the survey in Google Forms with anonymous response collection, a clear participant information statement at the top, and a "prefer not to say" option on demographic questions. Distributed the link through student WhatsApp groups, class chats, and direct outreach.

**Data collection.** Collected three valid responses during the two-day pilot window. All responses are anonymous; no identifying information was captured. The module is framed as a pilot study, so the small sample is a defined feature of scope rather than a data-collection failure.

**Analysis.** Built a six-sheet Excel workbook (Instructions, Raw_Data, Analysis, Demographics, Barriers, Summary) with formulas that automatically compute descriptives, agreement percentages, frequency distributions, and demographic breakdowns from the raw data. Generated bar charts for mean Likert scores, barrier frequency, and preferred campaign format. Converted Likert text responses (e.g. "Agree") to numeric values 1 to 5 in the Raw_Data tab so that all downstream statistical formulas would compute correctly.

**Writing.** Completed a full research report covering abstract, introduction, methodology, preliminary findings, discussion (including limitations), proposal, next steps, and conclusion. Findings sections reference the actual numbers computed on the Summary tab of the analysis workbook.

**Proposal.** Designed a Mental Health Resource Hub for the SafeX platform, built around three principles drawn directly from the findings: anonymity (as the primary entry point), visibility (of institution-specific resources), and stigma reduction through peer normalisation. Included a small complementary feature acknowledging the counsellor role-conflict issue raised in one open-text response. Included a three-phase implementation plan and an evaluation approach using follow-up survey comparison.

**Documentation.** Wrote a README covering the module purpose, repository structure, how it works, how to view or reproduce the analysis, and the tools used.

**Video.** Prepared an explanation video script covering architecture, tools, challenges, findings, and a working demo, structured to meet the 5 to 15 minute HD requirement with face visible throughout.

**Repository.** Set up the GitHub repository with all deliverables organised per the submission requirements.

## Key preliminary findings

- Two of three respondents (67%) reported that their institution offers mental health support.
- Mean self-rated awareness on a 1 to 5 scale was 3.00 (moderate).
- Two of three (67%) agreed that "seeking help for mental health is seen as a sign of weakness among students here."
- Only one of three (33%) said they would feel comfortable using their university's counselling service.
- Top primary barrier: fear of being judged by peers (67%). Second: cost or financial concerns.
- Top preferred campaign format: anonymous helpline or chat (67%). Second: social media content.
- One respondent identified a structural role-conflict issue in psychology departments where counsellors are also classroom teachers, undermining perceived confidentiality.

The direction across the closed and open items is consistent: within the surveyed group, the leading barrier to seeking mental health support is stigma and perceived judgement, not lack of information.

## Group coordination

Confirmed with the other members of Group 43 that my module (the awareness gap, stigma finding, and initiative proposal) does not duplicate any other member's work. My module sits alongside their contributions on the broader SafeX research project.

## Challenges encountered

**Response rate.** Distributing a mental-health-topic survey within a two-day pilot window produced a small sample (N = 3). Framing the study explicitly as a pilot from the outset was the correct methodological choice: the analysis pipeline, instrument, and proposal all remain valid at any sample size, and the workbook is designed to scale.

**Sensitive topic handling.** Question wording required particular care so that respondents were not asked to disclose their own mental health difficulties. All items were phrased in general awareness and attitude terms rather than personal disclosure, which is more appropriate for an awareness study.

**Analysis pipeline reusability.** Balancing a workbook that is easy to update (paste responses, everything recomputes) against one that is transparent to a reader. Solved by adding an Instructions tab, converting Likert text to numeric 1-5 explicitly in the Raw_Data tab, and using formula references throughout.

## Deliverables submitted

- Raw anonymised survey data (Excel workbook, Raw_Data tab)
- Written report (DOCX and PDF)
- Working files: Google Form (live link) and Excel analysis workbook
- Written documentation (README.md)
- Screenshots of the form and the analysis
- Explanation video (link in Video_Link.txt)
- This progress report
- Group Leader feedback form to be submitted separately by Friday, per the brief

## Next steps

The module is complete for Week 2. If the initiative moves forward beyond this submission, natural next steps would be a scaled deployment of the same instrument to a larger, more representative student sample, followed by a proof-of-concept build of the Mental Health Resource Hub at one partner institution. Re-administration of the survey after that deployment would enable direct measurement of change on the stigma and comfort items.
