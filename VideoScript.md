# Video Explanation Script

**Presenter:** Yashal Manaiem Javaid
**Module:** Mental Health Awareness Research, Week 2 individual contribution
**Group:** 43, SafeX Solutions Research Project
**Target length:** 8 to 10 minutes
**Format:** HD, face visible throughout, screen-share during the demo section

---

## Required coverage (from the brief)

Every section below is tagged with what part of the brief it satisfies:
- **[ARCH]** = architecture
- **[TOOLS]** = tools used
- **[CHAL]** = challenges
- **[DEMO]** = working demo

---

## [0:00 to 0:40] Introduction

Hi, I'm Yashal Manaiem Javaid. I'm a BS Psychology student at COMSATS University Islamabad, currently in my third semester, and this video is my Week 2 individual contribution to Group 43's SafeX Solutions research project.

The module I built is called Mental Health Awareness Research, and it's structured as a pilot study. I'll explain what that means in a moment. Over the next few minutes I'll walk you through what I built and why, the tools I used, the architecture of the module, the challenges I ran into, and then I'll actually show you the survey and the analysis working end to end. At the end I'll cover what the pilot data tells us and the initiative I'm proposing for the SafeX platform based on those findings.

---

## [0:40 to 1:40] Why this module

Mental health is a topic I care about both academically and personally. As a Psychology student, one of the first things you learn is that there is often a very wide gap between the number of people who need mental health support and the number who actually seek it. That gap has many possible causes: stigma, cost, cultural factors, not knowing where to go. If you want to design an intervention that actually works, the first thing you need to do is figure out which of those causes matters most in your specific population.

That is what this module is about. Rather than assuming what students need, I designed a survey to ask them directly: do you know that mental health support exists at your institution, do you feel comfortable using it, do you feel comfortable talking about mental health with peers, and what is the single biggest thing stopping you from reaching out?

I framed this deliberately as a pilot study. Within a single Week 2 module it's not realistic to collect a large, nationally representative student sample, and it would be misleading to pretend otherwise. So instead, the module delivers three things: a validated survey instrument, a working analysis pipeline built in Excel, and a set of preliminary observations that can guide the proposal. If SafeX or anyone else wants to scale this later, everything is set up to run again with a bigger sample.

---

## [1:40 to 3:00] Architecture and tools **[ARCH] [TOOLS]**

The module has three connected components. I want to walk through how they fit together because the design was deliberate.

The **first component** is data collection. I built an anonymous Google Form with three sections: demographics, awareness and attitudes (including four Likert-scale statements), and a barriers and preferences section that also included two open text questions. The form was distributed through student WhatsApp groups and class chats. Google Forms was the required tool for this module, and it worked well because students are comfortable filling out a form on their phone.

The **second component** is analysis. Once the responses were in, I exported them to Microsoft Excel. I built a six-sheet analysis workbook where the raw data goes into one tab, and every other tab updates automatically through formulas. That means if this pilot is ever scaled up, the workbook doesn't need to be rebuilt; someone at SafeX can just paste in fresh data and get the same analysis. I used standard statistical functions like COUNTIF, AVERAGE, MEDIAN, and MODE, along with bar charts.

The **third component** is the output layer: a written research report in Microsoft Word, this explanation video, and the whole thing hosted on GitHub as the project repository.

So the flow is: Google Form collects the data, Excel analyses it, Word turns the analysis into a report and a proposal, and GitHub hosts everything. Simple, but each piece has a job.

---

## [3:00 to 4:00] Challenges **[CHAL]**

I want to be honest about the challenges, because there were a few.

The **first challenge** was that this is a sensitive topic. Getting students to respond to a mental health survey requires them to trust that their answers really are anonymous, and that the survey isn't going to ask them to disclose their own difficulties. I handled that in two ways. I added a clear participant information statement at the top of the form explaining that responses were anonymous, voluntary, and that no personal information would be collected. And I phrased every question around awareness and attitudes rather than personal disclosure, so I was asking students what they think, not what they've experienced.

The **second challenge** was response rate within a Week 2 timeline. Recruiting a large student sample in a few days is genuinely hard, and my pilot ended up at three responses. This is one of the reasons I framed the study as a pilot from the beginning rather than as a definitive study. The pilot framing is honest about what a single-week module can and can't deliver, and the analysis is designed to remain valid at any sample size.

The **third challenge** was designing an analysis workbook that would still be useful to someone who isn't me. If I hardcoded the numbers, the workbook would be a one-time artifact. So I built it around a single paste-and-update flow, where the entire analysis updates from one tab of raw data. That took longer to set up but it made the deliverable much more reusable, which matters if this pilot ever gets scaled up.

The **fourth challenge** was making sure my module didn't duplicate what other members of Group 43 are doing. I coordinated with the group so that my angle, the awareness gap and the intervention proposal, sits alongside their contributions rather than overlapping.

---

## [4:00 to 6:00] Working demo **[DEMO]**

*[Switch to screen share for this section]*

Let me show you the module actually working.

*[Show the Google Form]* This is the Google Form. You can see the participant information statement at the top explaining that responses are anonymous. The first section is demographics: level of education, academic field, and gender, all with a "prefer not to say" option. The second section covers awareness and attitudes, including four Likert-scale statements running from Strongly disagree to Strongly agree. The third section covers barriers, preferred channels, and open feedback.

*[Show the Google Forms Responses tab]* Here on the Responses tab you can see the three responses that came in during the pilot. The form exports them straight to Google Sheets, and from Sheets I download an .xlsx file.

*[Switch to Excel, open the analysis workbook]* This is the analysis workbook. The Instructions tab explains the workbook and how to scale it later. The Raw_Data tab is where the exported responses live, with the Likert answers converted from text to numbers 1 through 5.

*[Click on the Analysis tab]* This tab is where the automation happens. It shows the mean, median, mode, and agreement percentages for every Likert item. All of these are formulas, nothing is hardcoded. To prove that, watch what happens if I temporarily remove a row from the raw data.

*[Go to Raw_Data, delete a row, come back to Analysis]* The numbers update. And when I undo that...

*[Ctrl+Z, return to Analysis]* Everything recomputes. That's what I mean when I say the pipeline is reusable. Pasting in a larger sample tomorrow would give you the same analysis structure automatically.

*[Show the distribution table and chart]* Below the summary is the full frequency distribution and a bar chart of the means.

*[Click Demographics tab, then Barriers tab]* Same principle here. The Demographics tab shows automatic breakdowns of the sample. The Barriers tab shows the barrier ranking and the preferred campaign format, both with charts.

*[Click Summary tab]* And this is the Summary tab, where the headline numbers used in my written report come from.

*[Switch back to camera]*

---

## [6:00 to 8:00] Preliminary findings and proposal

Now to what the pilot data actually tells us. I want to be careful here because the sample is small, so I'm reading these numbers for the direction they point in, not as definitive population estimates. And what they point to is genuinely interesting.

Two of my three respondents, so about 67%, said their institution offers mental health support. Self-rated awareness averaged 3 out of 5. So students in this sample largely know that support exists.

But knowing it exists isn't the same as feeling able to use it. Only one of three respondents, 33%, said they would feel comfortable using their university's counselling service. Two of three (67%) agreed that seeking help for mental health is seen as a sign of weakness among students. And when I asked directly what the biggest barrier to seeking help was, two of three respondents (67%) selected "Fear of being judged by peers." No one selected "don't know where to go."

So the story here isn't an information gap. It's a stigma gap. Students know support exists; what stops them using it is fear of being seen using it.

That fits with another finding. When I asked what format students would most likely engage with, two of three (67%) chose anonymous helpline or chat, and the third chose social media content. Nobody picked in-person workshops, peer support groups, or guest speakers. They want anonymous entry points.

The open text responses added something I couldn't have gotten from the closed items. One respondent, a psychology student, wrote that most of their department's counsellors are also their teachers, which creates bias inside the classroom. That's a really sharp observation. It's a structural role-conflict problem that no awareness campaign alone can fix, but it explains why anonymity matters so much to these students.

So the proposal I'm making to SafeX is a Mental Health Resource Hub built around three principles that come directly from this data. First, anonymity: an anonymous self-check tool students can use without creating an account, plus an anonymous helpline or chat function. This is the primary entry point because it addresses the leading barrier. Second, visibility: a searchable, institution-specific directory of who to contact and how, because even where support exists, information about it is still moderate at best. Third, stigma reduction through peer normalisation: short peer-produced content from students who have sought help before, presented anonymously by default. Peer testimony is one of the most reliably effective interventions for shifting perceived social norms.

I've also included in the report a small feature acknowledging the role-conflict issue: a section within the hub that transparently notes structural realities of on-campus support and points to external anonymous options for students who feel their institutional setup affects their confidentiality.

The evaluation approach is to re-administer this same survey a semester after launch and measure whether stigma agreement drops and comfort using formal support rises.

---

## [8:00 to 8:45] Deliverables and closing

Everything I've talked about is in the group's GitHub repository: the survey instrument, the anonymised pilot data, the Excel workbook, the written report, this video's script, and the README explaining how to view or reproduce the module. Because everything is set up to run again with a larger sample, this pilot has real reuse value beyond the Week 2 submission.

To close: what the pilot data tells us is that when it comes to student mental health awareness, the biggest problem in this sample isn't that students don't know help exists. It's that they don't feel able to use it. The proposal I've put forward is designed to lower the visibility cost of taking a first step, and it's structured so that its impact can actually be measured.

Thank you for watching. I welcome any feedback from the group and from the module coordinators.

---

## Delivery notes

- **Pace:** aim for around 130 to 140 words per minute. This script is calibrated to land in the 8 to 10 minute range at that pace.
- **Recording setup:** face visible throughout, HD (1080p minimum). Good lighting on your face; camera at eye level.
- **Screen share:** for the demo section (4:00 to 6:00), share your screen and walk through the actual form and Excel workbook. The delete-a-row / undo demo at 4:30 is the moment that proves the workbook is live, not hardcoded. Do that clearly on camera.
- **Rehearsal:** read aloud once end-to-end before recording. The tone should be professional but not stiff. You know this topic well as a Psychology student, so let that come through.
- **Numbers to remember:** the report and this script are already filled in with your actual numbers (67% aware of support, 67% see stigma, 33% comfortable using counselling service, top barrier is fear of judgement, top preferred format is anonymous helpline/chat).
- **Upload:** Google Drive is easiest. Right-click uploaded video, Share, Anyone with the link, Viewer. Paste link into `Video_Link.txt` in the repo.
