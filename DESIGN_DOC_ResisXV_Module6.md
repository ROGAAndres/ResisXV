# Product Agent Design Doc

<!-- DO NOT EDIT THIS HEADER BY HAND. Claude updates it on every "record" command. -->
**Venture:** ResisXV
**Student name(s):** Andres Rojas
**Last updated:** November 12 2026
**Modules recorded:** 3, 4, 5, 6 (Module 6 recorded to date; assignment tasks remain open)
**Tools on record:** 22 documented workflows (3 from Module 3; 7 from Module 4; 7 from Module 5; 5 from Module 6); no operational lodging integration claimed

---

## How this document works

This is your running record of every tool you build this semester. You do not write in it directly. At the end of each weekly session in this Project, type:

> record for module N in design document

Claude reads the session, drafts the entries for that module, asks you for anything it cannot find, and returns a new copy of this file. Download it and replace the old DESIGN_DOC.md in the Project's files. That is the whole loop.

Three rules Claude follows, and you should expect:

1. Nothing gets invented. If a field was not discussed in the session, Claude asks you before writing it.
2. Old entries are never rewritten. If a later week changes an earlier tool, a dated line goes under that tool's **Revisions**.
3. Every field gets filled. Two are easy to skip and are graded hardest: **Alternative considered and rejected** and **Honest limits**. A tool with no stated limits has not been thought through.

For any tool whose job is to judge or challenge something (a grill pass, a steelman challenge, a red-team pass, a consistency checker), **Success criteria** must include a demonstrated case proving the tool responds to what it is actually given. For a pass/fail tool, show it failing something. For a tool that generates critiques, show two different inputs producing materially different output.

---

## Project Scaffolding

One live scaffold. Claude updates it in place as files and folders are added. It should always show the project's current state, not a per-week log.

If your team works in Claude Projects rather than a file system, the named files in your Project knowledge stand in for folders. The logical structure matters, not whether it is a real directory.

```
ResisXV/
  project-context/
    DESIGN_DOC_ResisXV_Module6.md
  research-and-mrd/
    MRD_ResisXV.md
    ResisXV_Module4_MRD_and_Personas.docx
    ResisXV_Visual_MRD.pdf
    Journey_ResisXV.md
    Open_Hypotheses_ResisXV.md
  user-stories/
    User_Story_Board_ResisXV.xlsx
    Happy_Path_ResisXV.md
  affinity-and-content/
    Affinity_Map_ResisXV.pdf
    Affinity_Themes_ResisXV.md
    Content_Model_ResisXV.html
  design/
    ResisXV_Wireframes_English.pdf
    Screen_Flow_ResisXV.md
    Mood_Board_ResisXV.pdf
    Visual_Design_Brief_ResisXV.md
  reusable-tools/
    Journey_Template_ResisXV.md
    Privacy_5C_Checklist_ResisXV.md
    Screen_Card_Template_ResisXV.md
    Usability_Test_Plan_ResisXV.md
    Visual_Review_Checklist_ResisXV.md
    Submission_Consistency_Check_ResisXV.py
  submission/
    ResisXV_Module4_Design_Document.pdf
    ResisXV_Module4_English_Documents.zip
  module5/
    MVC_ResisXV.md
    Scrum_Board_ResisXV.xlsx
    Release_Plan_ResisXV.md
    Journey_Walkthrough_ResisXV.html
    Journey_Workflow_ResisXV.xlsx
    ResisXV_Final_MRD_Module5.docx
    User_Story_Board_ResisXV_Module5.xlsx
    ResisXV_Final_Wireframes_Module5.pdf
    Decision_Log_ResisXV_Module5.md
    ResisXV_Module5_Design_Document.pdf
  module6/
    PRD_ResisXV.md
    PRD_ResisXV.docx
    PRD_ResisXV.pdf
    Positioning_ResisXV.md
    GTM_Checklist_ResisXV.md
    DESIGN_DOC_ResisXV_Module6.md
    ResisXV_Module6_Design_Document.pdf
```

---

## Module 1: Idea and Vision

**Status:** not recorded
**Session date:**
**Summary (2 to 3 sentences on what the team did this week):**

### Tool 1.1
- **Name:**
- **Job:** What repeatable task does this replace?
- **Architecture choice:** One-shot prompt, Skill, agent with memory, or workflow, and why this one.
- **Input:**
- **Output:**
- **Human checkpoint:** Where does a person have to check the output before it is trusted?
- **Success criteria:** How would you know if this got it wrong?
- **Alternative considered and rejected:**
- **Honest limits:** What does this tool deliberately not check or do?
- **Revisions:**
  - (none)

### Tool 1.2
- **Name:**
- **Job:**
- **Architecture choice:**
- **Input:**
- **Output:**
- **Human checkpoint:**
- **Success criteria:**
- **Alternative considered and rejected:**
- **Honest limits:**
- **Revisions:**
  - (none)

---

## Module 2: Opportunity Brief

**Status:** not recorded
**Session date:**
**Summary:**

*(tool entries added on record)*

---

## Module 3: Personas and Research

**Status:** recorded; research preparation and MRD drafting completed, primary fieldwork pending
**Session date:** October 15 2026, America/Matamoros
**Summary:** Developed ResisXV's worker persona, five testable hypotheses, two interview guides, an evidence scoreboard and a preliminary MRD. The student challenged the financial realism of hotels and supplied work and travel premises; subsequent research refined the claim from absence of accommodation to possible unaffordability. No interviews, willingness-to-pay results or employer agreements were fabricated.

### Tool 3.1
- **Name:** ResisXV MRD drafting and evidence workflow
- **Job:** Turn a product objective, persona assumptions and available evidence into a structured first MRD and an explicit development recommendation.
- **Architecture choice:** A human-reviewed chat workflow combining structured drafting, source retrieval, an evidence scoreboard and document generation. This was the workflow actually used; the class mrd-builder skill was unavailable in this session and has not been installed or edited.
- **Input:** Existing ResisXV objective; Jose Martinez persona; the supplied class MRD outline, Fiddler example and Beauty on Demand hypotheses; the assignment rubric; the student's highlighted Word comments; and official contextual research.
- **Output:** ResisXV_Module3_Corregido.docx: problem-led vision, persona, unmet needs, five hypotheses, guides, evidence, research plan, three interview questions, alternatives, use scenarios, risks, conditional recommendation and proposed skill instructions. The supporting packet follows this record in the submission PDF.
- **Human checkpoint:** Check that the venture remains occasional near-work accommodation; verify personal details, actual budgets, routes and quotes; review source dates; and approve priorities before relying on the draft.
- **Success criteria:** Include every first-draft section in the Canvas rubric; distinguish student inputs, sourced context and modeled assumptions; retain zero primary interviews; and link the recommendation to missing evidence. Demonstrated revision: the initial draft described hotels as alternatives without a budget comparison; after the student's objection, the revised draft added an affordability test and cost sensitivity rather than claiming that shorter travel proves demand.
- **Alternative considered and rejected:** A polished completed MRD that treats all hypotheses as validated. Rejected because no interviews or paid trials exist and regional statistics cannot validate individual demand. Full accommodation commitments were also rejected at this stage.
- **Honest limits:** Does not establish Jose's income, route, sleep loss, family acceptance or willingness to pay. The market sizing example is arithmetic rather than a verified TAM. The official class skill and lab slides were not available; proposed categories and thresholds are not claimed to reproduce their wording.
- **Revisions:**
  - October 15 2026: Incorporated the student's affordability objection and work schedule; added sourced contextual evidence, counterevidence and an explicit worked example.
  - October 22 2026: Module 4 revises the current persona to I1, incorporates supplied summaries and creates English MRD/visual outputs. The Module 3 snapshot is retained.

### Tool 3.2
- **Name:** ResisXV discovery interview preparation workflow
- **Job:** Convert uncertain customer and buyer assumptions into neutral, traceable research questions and a consistent notes structure.
- **Architecture choice:** Reusable guide drafted through a structured chat workflow, with separate worker and employer audiences. No persistent interview agent or installed discovery-interviews skill was used.
- **Input:** Five H IDs, worker persona, possible employer buyer, JTBD framing and the requirement to explore past behavior before introducing a concept.
- **Output:** Two 20-minute guides with introduction, exploration, validation and conclusion; recruitment and consent fields; question-to-hypothesis links; top three worker questions; and an interview notes schema.
- **Human checkpoint:** Recruit appropriate participants, disclose relationships, obtain consent, ask neutral probes, record accounts faithfully and distinguish direct quotation from paraphrase. Review whether income questions are necessary and comfortable for the participant.
- **Success criteria:** Questions explore actual decisions and alternatives before concept reaction. Demonstrated audience adaptation: worker inputs produced questions about the last commute, recovery and household tradeoffs; employer inputs produced questions about staffing evidence, purchasing authority and approval routes. Neither guide uses positive concept reaction as payment validation. Actual research quality remains untested because neither guide has been fielded.
- **Alternative considered and rejected:** One identical guide for workers and employers. Rejected because the user of accommodation and the possible purchaser have different jobs and constraints. Invented or AI role-played interviews were rejected as a substitute for research evidence.
- **Honest limits:** A prepared guide is not an interview. There are no respondent quotations, recruitment records, findings, invalidated hypotheses or interview-based opportunity scores to report. Two future interviews would provide early qualitative reads, not market prevalence.
- **Revisions:**
  - October 15 2026: Added route, working-day, household-budget and actual-quote probes after the student's highlighted comments.
  - October 22 2026: Four source summaries are now available in Module 4. The worker guide and proposed employer follow-up are distinguished; exact dates and relationships remain open.

### Tool 3.3
- **Name:** Premise and evidence challenge pass
- **Job:** Identify claims that exceed the evidence and replace them with sourced findings, explicit assumptions or testable questions.
- **Architecture choice:** A human-reviewed challenge workflow using highlighted comments, web research and transparent calculations. Chosen because factual support, affordability arithmetic and customer validation require different checks.
- **Input:** The student's claims about hotel affordability, an 8:30 a.m. to 5:30 p.m. schedule and approximately 48 weekly hours, bus and Metro travel, potential time savings, safety concerns and family acceptance.
- **Output:** Revised framing and evidence scoreboard; a validation checklist; and a modeled stay-cost and time comparison. Sources include INEGI EOD 2017, INEGI ENVIPE 2025, CONASAMI's 2026 wage resolution and official hotel pages.
- **Human checkpoint:** Confirm source freshness and scope. Obtain current lodging quotes and individual budgets; do not attribute minimum-wage income to Jose. Verify actual workdays and breaks before deriving weekly hours.
- **Success criteria:** A claim fails if it treats inference as observation or ignores material counterevidence. Demonstrated contrast A: "there is no hotel alternative" failed because official local hotel pages show supply, so the output became an affordability hypothesis. Contrast B: "accommodation exists but may not fit disposable income" was retained as testable; the output requested dated quotes, household budgets and paid choices rather than rejecting supply. Calculation check: two 90-minute long journeys replaced by two 20-minute local journeys yield 140 minutes recovered, not an automatic three hours of extra sleep.
- **Alternative considered and rejected:** Treating a plausible Mexican-worker example as completed interviews or applying a general assumption about Mexican family behavior. Rejected because a model cannot establish observed customer experience, and household obligations differ.
- **Honest limits:** Hotel Panorama's advertised MXN 250 rate is undated and not a confirmed current quote. ENVIPE's 85.2% figure is perceived public-transport insecurity among adults in the State of Mexico, not a route-level crime probability. Official wages are contextual benchmarks; scenario costs and household choices remain assumptions.
- **Revisions:**
  - October 15 2026: Incorporated supporting and conflicting evidence and replaced all highlighted drafting prompts with final text.
  - October 22 2026: Later research applies student budget corrections. Current company-wide funding and paid feasibility remain unverified; prior contextual sources are not refreshed by this record.

### Research outputs and current decisions

**Vision:** Workers with long commutes should be able to protect recovery and reliable arrival without destabilizing their household. ResisXV explores occasional accommodation near work while preserving the worker's main home.

**Primary persona:** Jose Martinez, 45, production floor supervisor at PEFSA, living in Chimalhuacan with his wife and two children. The student reports an 8:30 a.m. to 5:30 p.m. schedule, approximately 48 hours per week, local surface transport plus Metro, and a three-to-four-hour daily commute. These remain project inputs rather than interview findings; exact workdays, breaks, income and routes require confirmation.

**Core unmet-need themes:** recovery and reliable arrival; affordable overnight alternatives while household expenses continue; and compatibility with family responsibilities. Safety and cleanliness are decision criteria to investigate, not established advantages of ResisXV.

**Five hypotheses and status:**
1. H1: Long travel reduces recovery between workdays. Future test: at least three of five diary participants lose an hour of intended rest on two workdays. Untested, primary n = 0.
2. H2: Existing overnight options can exceed available household budget. Future test: at least three of five workers identify a real need but reject a dated quote for a documented budget reason. Untested, primary n = 0.
3. H3: Household obligations can block occasional overnight adoption. Future test: at least three of five workers identify a specific use occasion with a workable household arrangement. Untested, primary n = 0.
4. H4: Added accommodation spending constrains self-pay demand. Future test: at least three of ten eligible workers voluntarily reserve a stay at a viable disclosed price. Untested, primary n = 0.
5. H5: Employer support depends on documented needs, budget and approval authority. Future test: one authorized employer agrees to a scoped pilot, with suitable supply assessed separately. Untested, primary n = 0.

**Evidence:** Historical EOD data supports investigating long work journeys; ENVIPE adds regional perception evidence; official wage and hotel information motivate an affordability comparison. None establishes product demand. Complete source links and limitations appear in the supporting packet.

**Additional research:** First conduct two worker interviews, then a separate employer interview. Follow with a five-worker travel and rest diary, at least three dated lodging quotes, budget comparisons and, only if feasible, a limited voluntary paid pilot. This is a proposed sequence, not completed or scheduled fieldwork.

**Top three interview questions:**
1. Walk me through your most recent workday, from leaving home to returning.
2. Tell me about the last time your commute affected your rest, work plans or responsibilities at home. What happened?
3. What have you tried to improve that situation, and how did you decide whether it was worth the time and expense?

**Recommendation:** Conditional Go for discovery and cost feasibility; No Go for accommodation commitments until affordability, worker demand, household fit, suitable supply and any employer approval are established. Proposed review date: October 29 2026, subject to arranging research; this is not a scheduled reminder or a promise that research will be complete.

### Student contribution and response to AI

The student's initial objection was that hotels were not economically realistic for the target worker. The student also supplied schedule and transport details and identified family acceptance as a concern. The revision treats affordability as a central constraint, uses current official wage context and checks actual accommodation supply; it replaces the unsupported absolute claim with a testable comparison. No additional student opinion or first-pass reasoning has been invented.

### Proposed harness revisions

**MRD instructions:** Define the role, objective and inputs; identify the top job before proposing scope; separate findings from assumptions; require evidence for and against every hypothesis; report n and verdicts; compare alternatives on customer hiring criteria; and use explicit development gates. With no primary research, retain untested verdicts and label all scenarios.

**Discovery instructions:** Separate worker and buyer guides; number questions to hypotheses; use neutral, open questions about past behavior; introduce the product only after exploration; disclose recruitment; and record limitations. Do not generate participant identities, quotations, completed notes or validation results.

**Iteration checks:** Re-run the challenge on an absolute claim and a qualified claim and confirm materially different outputs. Check time and cost arithmetic, source dates, research denominators and hypothesis links. These are documented proposed revisions, not proof that the class skills were uploaded or modified in Claude.

### Files and handoff

- ResisXV_Module3_Corregido.docx: supporting research and MRD packet.
- DESIGN_DOC_ResisXV_Module3.md: updated running record; replace the old project-context design document with this file.
- ResisXV_Module3_Submission.pdf: updated design record followed by the supporting packet for review and Canvas submission.
- Remaining gaps: real interviews and synthesis; confirmed class-skill installation and invocation; verified personal budget and route; actual paid demand.

---

## Module 4: User Stories

**Status:** recorded; deliverables drafted and exported, research and operational limits disclosed
**Session date:** October 22 2026, America/Matamoros
**Summary:** Converted supplied interview summaries into an updated persona-led MRD, twenty primary stories plus three internal proposals, an affinity map, an eleven-type content model and eleven static wireframes. The student supplied the moodboard, corrected the individual versus company-wide funding scope and the I4 nightly budget, and requested all submission documents in English. This session documents completed drafting and reusable workflows; it does not claim funded accommodation, completed stays, usability findings or an externally submitted assignment.

**Recording scope:** This entry was prepared in ChatGPT Work from the ongoing project. The original course template's references to Claude are retained as template instructions, not a claim that the work ran in Claude. The earlier Module 3 entry was restored verbatim from DESIGN_DOC_ResisXV_Module3.md and remains a dated snapshot; its current-state assumptions are superseded below.

### Evidence and decisions carried forward

- Primary persona: Sebastian I1, an operational worker living in Chimalhuacan and working around Barranca del Muerto. The earlier Jose/PEFSA persona remains in the Module 3 historical entry only.
- Research basis: four supplied source records, I1/I3/I4 worker accounts and I2 employer stakeholder. I4 is labelled Jocelyn / Manolo and unique identity/count remains unresolved. Counts are source records, not market prevalence. Notes consent is reported; exact dates and precise recruitment relationships still need completion.
- I2 correction: MXN 3,000-4,000 weekly for the entire company. Approximately MXN 12,000 monthly is a working estimate requiring reconciliation, not an additional funded commitment. I2 is not established as I1's employer.
- I4 correction: MXN 100 per night is the stated limit, not MXN 500, a payment or a viable service price. The unreconfirmed monthly amount is excluded.
- Student-originated concern: decide who can receive scarce support and consider the effects on workers who cannot self-pay and receive no allocation. Eligibility, priority and review rules remain open.
- Canonical English journey: Plan, Recognize, Check, Review, Request, Reflect. It has context before a trigger and labelled hypothetical later-use stages. The gate passed for structure only.
- Recommendation: Conditional Go for prototype testing and supply/cost feasibility; No Go for paid stays or capacity commitments until funding, supply, voluntary choice and operating gates are resolved. October 29 2026 is a proposed review date, not completed work or a scheduled commitment.

### Tool 4.1
- **Name:** Interview observation coding and affinity synthesis
- **Job:** Turn supplied interview summaries into source-linked observations and a small set of research themes.
- **Architecture choice:** Human-reviewed workflow using the PM101 affinity-map skill. Source IDs remain stable so later stories can be traced to evidence. It uses the supplied notes rather than an autonomous interviewer.
- **Input:** Interview.html, four supplied source records I1-I4, student corrections to I2 and I4 budgets, and O01-O40 in the evidence ledger.
- **Output:** Forty paraphrased observations, eight proposed clusters, five themes T1-T5, an orphan observation O40, Affinity_Map_ResisXV.pdf and Affinity_Themes_ResisXV.md.
- **Human checkpoint:** Confirm observation meaning, clustering, interview dates and recruitment relationships. Clarify whether I4 is one person. Do not count an employer report about workers as additional worker interviews.
- **Success criteria:** Every observation retains its source; counts refer to records; contradictory accounts remain visible. Demonstrated contrast: I1 cannot self-pay, I3 excludes recurring accommodation and I4 has a corrected MXN 100 nightly limit. The synthesis distinguishes these accounts instead of reporting one shared willingness-to-pay figure.
- **Alternative considered and rejected:** Rationale recorded now: a single positive summary of all interviews was not used because it would hide household and payment differences. Forcing every observation into a theme was not used; O40 remains an open family-emergency question.
- **Honest limits:** Summaries are not transcripts and observation counts are not prevalence. I4 identity/count and timing remain uncertain. No paid stay, rest outcome or causal attendance effect was established. Affinity columns retain earlier provisional stage labels; a full regeneration against the canonical English journey is still pending.
- **Revisions:**
  - October 22 2026: Applied the student correction that MXN 3,000-4,000 weekly is company-wide and that I4 states MXN 100 per night; removed reliance on the unreconfirmed monthly I4 amount.

### Tool 4.2
- **Name:** Evidence-led persona and visual MRD workflow
- **Job:** Revise the research persona and turn the MRD into a journey, evidence, data, metric and decision handoff.
- **Architecture choice:** PM101 MRD visualizer plus document-generation workflow, with an explicit journey gate and human review. A structured workflow was used because research evidence and proposed design must remain distinguishable.
- **Input:** Prior Module 3 MRD; I1-I4 summaries; five hypotheses; affinity themes; the reviewed six-stage journey; the course Apple accident teaching case; and the Canvas rubric.
- **Output:** ResisXV_Module4_MRD_and_Personas.docx; thirteen-slide ResisXV_Visual_MRD.pdf and MRD_Visual_ResisXV.html; Journey_ResisXV.md; Open_Hypotheses_ResisXV.md; Journey_Template_ResisXV.md; and Privacy_5C_Checklist_ResisXV.md.
- **Human checkpoint:** Review the move from the assumed Jose/PEFSA profile to Sebastian I1 around Barranca del Muerto. Check all n values and the company-wide funding scope. Treat the six-stage structural gate as a design check, not validation of real behavior after requesting.
- **Success criteria:** The journey begins before app use, names a trigger and ends in reflection. Each stage has a job, a source/n or a labelled hypothesis, and data. Demonstrated contrast: I1 home-life understanding and I3 nightly household duties produce different persona implications. Recommendation stays Conditional Go for prototype/feasibility and No Go for paid stays while operating gates remain unresolved.
- **Alternative considered and rejected:** The earlier Jose-primary, n = 0 draft was not retained as the current research persona once the user selected I1 and supplied summaries. A confident Go based on interest alone was not used. Opportunity ranks were kept qualitative because importance/satisfaction scores were not collected.
- **Honest limits:** One source record per profile is not saturation; I4 identity is unresolved. No defensible market-wide TAM, approved subsidy, supplier quote, paid demand or measured sleep improvement exists. The 50/30/20 diagnostic review weights and 50/80 bands are guesses and must never allocate worker support. Proposed dates are research-review targets, not completed research.
- **Revisions:**
  - October 22 2026: Superseded current n = 0 claims with four source records, keeping the earlier Module 3 snapshot as history.
  - October 22 2026: Produced an English document set and labelled scores, conditions, provider data and future outcomes as proposals.

### Tool 4.3
- **Name:** Persona-specific user story board and happy path
- **Job:** Convert the worker job and research constraints into design stories, traceability and a limited prototype scope.
- **Architecture choice:** PM101 user-story-board skill followed by human review and HTML/XLSX generation. The spreadsheet supports filtering and later edits; the happy-path Markdown is a reusable wireframe input.
- **Input:** Sebastian I1; the six journey stages; T1-T5; H1-H5; three proposed epics; and the twenty stories reviewed in chat.
- **Output:** Twenty primary stories S01-S20 and three separate internal proposals A01-A03 in User_Story_Board_ResisXV.xlsx, .html and .md; Happy_Path_ResisXV.md. Ten prototype P0 stories are proposed, including S12/S15/S16 exceptions.
- **Human checkpoint:** Check that every story has role, situation, motivation and a distinct outcome. Review the proposed MVP and any later scope expansion separately from accepting the story wording. Do not treat all interface emotions as interview observations.
- **Success criteria:** At least twenty primary stories, at least two per stage, at least three unhappy-path stories and three internal stories outside the primary count. The recorded structural check finds 20 primary, 3 internal and all prototype P0 IDs on screen cards. The user accepted the twenty as a draft; this does not validate their adoption assumptions.
- **Alternative considered and rejected:** Rationale recorded now: a feature checklist or twenty identical happy-path requests would not express situations, worker outcomes or escape paths. An all-P0 board was not used; v1 and Later retain lower-priority work.
- **Honest limits:** The happy path and ten-story MVP are design proposals. P0 means prototype priority; linked hypotheses are not all validated. Internal roles were proposed without separate interviews. W02/W06/W08 add explanation, timing and closing-cost detail beyond the original MVP tags; these changes are disclosed rather than silently treated as approved scope.
- **Revisions:**
  - October 22 2026: Organized the accepted stories into a board and exported the seven-step happy path plus three critical exceptions.
  - October 22 2026: Converted the submission edition, including headers and metadata, to English at the user request.

### Tool 4.4
- **Name:** Story-to-content model and coverage workflow
- **Job:** Identify the information each story requires and define its source, ownership, lifecycle, relationships and calculations.
- **Architecture choice:** PM101 content-model skill with a structured dictionary, relationship diagram and story coverage check. A content model was used before treating screen labels as real available data.
- **Input:** The story board, journey, affinity themes, funding correction and later screen cards. No live provider integration or operational database was supplied.
- **Output:** Content_Model_ResisXV.html and .md; eleven proposed content types; typed fields and sources; relationships/cardinalities; budget, copay, inventory and outcome formulas; and a reusable content-type template section.
- **Human checkpoint:** Confirm every field and who can change it. Resolve administrative capture of required fields, budget-period rules, inventory expiry and consent/retention before implementation. Confirm each visible field against a screen card.
- **Success criteria:** All 23 story rows have a structural read/write mapping and all eleven types have an ID, creation timestamp and status. The budget formula counts each allocation once in its current state, and copay is total minus support. Missing data yields no outcome score; it is not silently converted to zero.
- **Alternative considered and rejected:** Rationale recorded now: buttons and screens were not modelled as data entities. A single employee-budget field was not used because the correction establishes a shared company fund. A large future-service model was not used; the draft stays below twelve types.
- **Honest limits:** Structural coverage is not a working system. The model does not establish price viability, physical capacity, safety or funding. All internal required-field capture has not passed a full screen/operations review. The weighted diagnostic score is read-only and provisional, not a funding rank.
- **Revisions:**
  - October 22 2026: Separated support program, allocation, request and stay records so company funds are not confused with personal entitlement.
  - October 22 2026: English edition carries formulas forward and includes the provisional diagnostic score with explicit limits.

### Tool 4.5
- **Name:** Low-fidelity wireframe and usability planning workflow
- **Job:** Show the chronological task, information, next action and explicit exit for the prototype worker journey.
- **Architecture choice:** PM101 wireframe/screen-flow skill using grayscale vector drawings, annotated cards and PDF/HTML export. Static files were chosen; no Balsamiq, Figma, Jira or Trello connection is claimed.
- **Input:** Happy_Path_ResisXV.md; story IDs; content fields; primary-persona constraints; and successive chat reviews of screen groups.
- **Output:** Eleven screens W01-W11 in ResisXV_Wireframes_English.pdf and Wireframes_ResisXV.html; Screen_Flow_ResisXV.md; Information_Architecture_ResisXV.mmd; Screen_Card_Template_ResisXV.md; and Usability_Test_Plan_ResisXV.md.
- **Human checkpoint:** Review groups of screens for understandable cost, pending versus approved state, and exits. W01-W06 received chat acceptance; later screens were delivered and work continued, without separate accept/edit/reject responses for every detail. Test with actual profile-matched workers before relying on comprehension.
- **Success criteria:** All ten prototype P0 stories appear on screen cards. Every screen names the task, next action, back-out, content and inferred emotion. Denial does not silently create self-payment; leaving does not cancel a submitted request; cancellation requires confirmation. A test plan specifies five prospective workers, neutral tasks, completion, seconds, errors, help and satisfaction.
- **Alternative considered and rejected:** The work used low-fidelity files rather than a polished branded interface or a live booking implementation. Login was not made the first job; the initial screen starts with the night and cost limit. Automatic support approval and automatic self-pay after denial were not used.
- **Honest limits:** The screens do not execute booking, payment, support decisions or access. MXN 180, zero copay, sample addresses, conditions, eligibility and times are fictional. Five usability participants have not been recruited and tests have not been run. No completed stay, measured usability rate or real approval is claimed.
- **Revisions:**
  - October 22 2026: Added explicit no-availability, rejection/review and cancellation states; combined the eleven drawings into one file.
  - October 22 2026: Recreated the eleven screens and cards in English after the user language instruction.

### Tool 4.6
- **Name:** Student moodboard review and reusable visual brief
- **Job:** Translate the student-supplied collage into a proposed emotional and visual direction for later interface styling.
- **Architecture choice:** PM101 mood-board skill used as a review and brief-writing workflow. The student supplied the images; no generated replacement imagery or new branded assets were needed.
- **Input:** Mood Board.pdf, I1 constraints, the affinity themes, Norman visual/behavioral/reflective levels and existing low-fidelity screens.
- **Output:** The original moodboard preserved unchanged; Visual_Design_Brief_ResisXV.md; and Visual_Review_Checklist_ResisXV.md. Proposed desired words are calm, trustworthy and dignified.
- **Human checkpoint:** The student should confirm the proposed stance/adjectives and decide whether to add type, per-image captions or a contemporary worker reference. Do not attribute those proposed refinements as decisions already made by the student.
- **Success criteria:** The review connects material/light references with rest and trust and keeps cost/state clarity at the behavioral level. It identifies the missing type specimen and captions rather than treating a collage as a complete interface specification. The existing historical-worker images are context cues, not research evidence.
- **Alternative considered and rejected:** Rationale recorded now: replacing the student board with generic AI imagery was not used. Luxury styling or competitor screen copying was not adopted as the product direction, because affordability and worker dignity are central constraints.
- **Honest limits:** The proposed stance and captions have not been fully endorsed, and suggested image/type refinements were not performed. The board does not prove room cleanliness or safety. The brief is not a final brand system or a tested interface.
- **Revisions:**
  - October 22 2026: User supplied the existing board; inventory changed from missing to received with minor refinements proposed.
  - October 22 2026: Added an English visual brief and checklist while preserving the source PDF.

### Tool 4.7
- **Name:** English handoff packaging and bounded consistency checker
- **Job:** Keep the document set understandable and catch basic ID, count and funding-scope errors before handoff.
- **Architecture choice:** PM101 packaging review plus a small reusable Python checker operating on structured story data and screen-card IDs. It is a bounded file workflow, not an autonomous grader or an installed new skill.
- **Input:** English MRD/personas, story JSON/XLSX, content model, screen cards, affinity map, moodboard and explicit company-wide funding scope.
- **Output:** ResisXV_Module4_English_Documents.zip; README_English_Set.md; Submission_Consistency_Check_ResisXV.py; and Submission_Consistency_ResisXV.json. This recording adds the completed Module 4 design document and PDF to the package.
- **Human checkpoint:** Review source facts and open consistency issues. A passing structured check cannot certify research or Canvas readiness. The student must upload the PDF and replace the design-document copy in project context.
- **Success criteria:** Eight bounded baseline checks passed on current inputs. A controlled negative input removed S13 from screen coverage and changed the structured funding scope to per-worker; the checker failed both rules and reported missing S13. Original submission files were not corrupted. This demonstrates input sensitivity, not validation of the venture.
- **Alternative considered and rejected:** A presence-only inventory was not considered sufficient: it cannot detect a missing P0 story or a wrong scope assertion. A full automatic score or unconditional ready-to-submit badge was not used because research metadata, legacy stage labels and operational field capture remain unresolved.
- **Honest limits:** The checker does not validate note authenticity, all narrative budget statements, every required field, visuals, live prices, safety, usability or a rubric grade. The legacy affinity-map columns are not fully aligned with the canonical English journey. The prior coaching scores use different denominators and are not summed into a claimed Canvas grade.
- **Revisions:**
  - October 22 2026: Built English submission editions after earlier Spanish drafts; the source interview records remain unchanged.
  - October 22 2026: Ran an actual passing baseline and a deliberate failing control while recording Module 4.

### Deliverables for the assignment

| Item | File or record | Current status |
|---|---|---|
| 1 Visual MRD | ResisXV_Visual_MRD.pdf; MRD_Visual_ResisXV.html; ResisXV_Module4_MRD_and_Personas.docx | Drafted in English; persona evidence and open hypotheses disclosed. |
| 2 User Story Board | User_Story_Board_ResisXV.xlsx; .html; .md | 20 primary stories and 3 internal proposals; prototype scope remains proposed. |
| 3 Moodboard | Student Mood Board.pdf; Visual_Design_Brief_ResisXV.md | Original received and reviewed; type/caption refinements remain proposed. |
| 3 Affinity map | Affinity_Map_ResisXV.pdf; Affinity_Themes_ResisXV.md | 40 observations, 5 themes and one orphan; legacy column labels need alignment. |
| 3 Content model | Content_Model_ResisXV.html; .md | 11 content types with sources, owners, relationships and formulas; full internal capture review pending. |
| 4 Wireframes | ResisXV_Wireframes_English.pdf; Wireframes_ResisXV.html; Screen_Flow_ResisXV.md | 11 static screens, including no availability, denial and cancellation; usability not tested. |
| 5 Design document | DESIGN_DOC_ResisXV_Module4.md; ResisXV_Module4_Design_Document.pdf | Recorded from this session; PDF exported for the student to upload to Canvas. |

### Bounded consistency review

The machine-check report has a passing eight-rule baseline and a deliberate failing control. The following broader review remains separate; it is not made true by the baseline result.

| Check | Result | Evidence or open issue |
|---|---|---|
| Primary research persona | Consistent by I1 reference; labels not word-for-word identical | MRD, story board and brief use Sebastian; screen cards cite I1 but do not always repeat the name. |
| Journey columns identical in every artifact | Open | Later English artifacts use the canonical six-stage set; the affinity map retains earlier provisional labels. Journey_ResisXV.md records the crosswalk, but the map was not fully regenerated. |
| Every prototype P0 on a screen and every cited story exists | Pass for structured IDs | Submission_Consistency_ResisXV.json baseline; negative control catches missing S13. |
| Screen types exist and required fields all have capture surfaces | Partial | The screen cards map displayed types/fields. Administrative required-field capture and authorization are not fully checked. |
| Affinity theme coverage | Present in the board | T1-T5 are cited. This checks linkage, not the validity or approval of the clustering. |
| Outcome computable from defined fields | Structurally mapped | Feedback rest/experience, stay actual copay and request accepted cap are defined. No completed-stay data exists; missing inputs mean no result. |
| Mood direction and trigger emotions | Proposed, not user-tested | Calm/trustworthy/dignified are intended responses to fatigue and uncertainty, not claimed participant feelings on app use. |
| MVP sentence and screen strip | Partially expanded with changes disclosed | The seven story steps are implemented through additional pending, condition and exception states. Some v1/Later details were pulled into the screen drafts; the board scope was not silently overwritten. |

### Actual iteration and student contribution

The student selected I1 as primary, challenged the I4 MXN 500 figure, corrected I2 funding to a company-wide pool, raised excluded-worker consequences, supplied the moodboard and required English documents. Early screen groups were reviewed in chat; later material was delivered for review. Alternative rationales labelled as recorded now are this recording's design explanation, not invented claims about a past student debate.

The central change is that travel burden, household fit and ability to pay are treated separately. Angélica's emergency-only situation contrasts with Sebastian's suggested weekday use; the prototype cannot assume that a shared company fund covers everyone. The user contribution is documented without claiming the student independently originated every AI-generated metric, field or screen.

### Remaining limits and next handoff

- Complete exact interview dates, prior relationships and I4 identity/count before treating the research metadata as complete. Do not fabricate missing values.
- Reconcile the company-wide weekly versus monthly funding estimate and obtain an authorized sponsor, rules and viable provider quotes before a paid pilot.
- Align affinity columns and confirm operational field capture before claiming full cross-artifact consistency.
- Test the prototype with five voluntarily recruited profile-matched workers; no usability results exist yet. Do not treat the static illustrations or fictitious MXN 180 price as transactions.
- Any source coaching scores are provisional and use different scales. No new aggregate score out of 100 or final Canvas grade is asserted here.
- Student handoff: upload ResisXV_Module4_Design_Document.pdf to Canvas and replace the old design-document copy in project context with DESIGN_DOC_ResisXV_Module4.md. This session does not claim those external uploads were performed.

### Reusable tools saved

Journey_Template_ResisXV.md, Privacy_5C_Checklist_ResisXV.md, Happy_Path_ResisXV.md, Screen_Card_Template_ResisXV.md, Usability_Test_Plan_ResisXV.md, Visual_Review_Checklist_ResisXV.md and Submission_Consistency_Check_ResisXV.py are included in the English handoff package. The checker has a recorded positive and negative input demonstration. These are files/workflows; no new installed skill or live third-party connection is claimed.

---

## Module 5: Customer Journey

**Status:** recorded; Module 5 artifacts prepared for student review and submission; research and live-use gates remain open
**Session date:** October 29 2026, America/Matamoros
**Summary:** Updated ResisXV from the Module 4 drafts into a complete story board, MVC one-pager, twelve-week delivery plan, actor-based customer workflow, final MRD and key wireframes. The student supplied the course skills and class examples, requested accurate matching of their structures, and directed motel/hostel comparison and English deliverables. Seven workflows are recorded below; this is a record of completed drafting and checks, not a claim that the product, research studies or funded accommodation operated.

### Current evidence and decisions

- Primary design persona remains Sebastián I1. The four supplied records comprise three worker records and one employer record, with I4 identity/count unresolved. Exact dates and prior recruitment relationships still need completion. No new interviews or quotes were generated as evidence.
- I2’s MXN 3,000-4,000 weekly range is for the whole company. It is not approved funding or a per-worker entitlement. The rough monthly estimate still needs a consistent period. I2 is not established as I1’s employer.
- The corrected MXN 100 nightly stated budget belongs to I4, not I1. Stated budgets do not establish a viable price or a payment.
- Canonical stages remain Plan, Recognize, Check, Review, Request, Reflect. Arrival and stay remain within Reflect. The proposed seven-stage split was not accepted and is not silently imposed.
- The student requested motel/hostel alternatives and supplied BOOST MVC and release-grid examples. Mobile web, managed hosting, occasional-one-night scope and numeric research thresholds are still proposals; authorization to draft is not evidence that every proposal was independently chosen or validated by the student.
- Conditional Go for research, supplier feasibility and controlled prototypes. No Go for paid operation while funding, supply, worker consent, responsible support and cost feasibility remain unresolved. The MRD proposes November 5 2026 as a review target; no appointment or reminder was created.

### Tool 5.1
- **Name:** User Story Board refinement
- **Job:** Connect worker, purchaser and internal needs to proposed releases.
- **Architecture choice:** Source-linked story register and spreadsheet/HTML exports; human review remains necessary.
- **Input:** Twenty worker and three internal Module 4 stories, purchaser additions P01-P05, the six-stage journey and the Module 5 release plan.
- **Output:** User_Story_Board_ResisXV_Module5.xlsx, .html, .md and .json; 28 stories with situation, motivation, outcome, emotion, behavior, evidence, hypothesis, epic, scope and release.
- **Human checkpoint:** Confirm purchaser authority, role-specific needs and proposed scope. I2 is not established as I1’s employer. Inferred emotions and unobserved purchaser behavior stay labelled.
- **Success criteria:** All 28 stories passed four-part wording checks, including grammatically correct “As an”; every stage has at least two worker stories. IDs match the Scrum register and all journey references.
- **Alternative considered and rejected:** Design rationale recorded in this pass: a worker-only board would omit the funding decision and spend justification. Five proposed purchaser stories were added; they are not claimed interview findings.
- **Honest limits:** No paid adoption is validated. P0 is a prototype dependency, not approval to ship. A01-A03 move explicitly from v1 to proposed MVP prerequisites. The full operations interface is not specified.
- **Revisions:**
  - October 29 2026: retained IDs, integrated purchaser stories and preserved original scope/change rationale; normalized non-worker stage labels while retaining source-stage metadata.

### Tool 5.2
- **Name:** MVC architecture one-pager
- **Job:** Translate stories and content into Model, Controller and View responsibilities.
- **Architecture choice:** A grayscale three-column one-pager patterned after the supplied BOOST example; not-headless mobile web and managed hosting are proposals.
- **Input:** Existing story board/happy path, eleven content types, worker and purchaser roles, BOOST MVC PDF and corrected course skills.
- **Output:** ResisXV_MVC_One_Pager.pdf, MVC_ResisXV.md/.html and MVC_Story_Trace_ResisXV.md. Six Model groups, eight Controllers and seven View groups.
- **Human checkpoint:** Review data ownership, employment verification, role restrictions, provider confirmation, copay acceptance and operating ownership before implementation.
- **Success criteria:** PDF verified as one landscape page. Every cited story ID resolves in the existing or proposed story supplement; controller/model links are explicit.
- **Alternative considered and rejected:** Native app deferred because the current occasional-stay stories establish no native-only requirement. A message-led concierge test can precede the proposed web product. These are design rationales, not a recorded student vote.
- **Honest limits:** No hosting vendor, integration, maintenance owner or retention policy is confirmed. A table cannot establish working authentication, atomic holds, privacy controls or commercial feasibility.
- **Revisions:**
  - October 29 2026: adopted the student’s BOOST structural benchmark and made the company-wide fund distinct from worker copay.

### Tool 5.3
- **Name:** Twelve-week Scrum Board and release plan
- **Job:** Sequence traceable work into weekly demonstrable outcomes and three releases.
- **Architecture choice:** One structured set of 58 cards rendered as a release-by-epic grid and weekly lists, with an Excel backlog and reusable Python linter.
- **Input:** MVC entries, the 28-story release register, happy path, class release-grid example and scrum-board-12-week instructions.
- **Output:** Scrum_Board_ResisXV.xlsx/.html, ResisXV_12_Week_Scrum_Board.pdf, Release_Plan_ResisXV.md, story register and Scrum_Card_Linter_ResisXV.py.
- **Human checkpoint:** Assign real people, capacity and a start date; review what each release proves and reduce scope if staffing cannot support the plan.
- **Success criteria:** Baseline structural checks passed for 58 cards and 12 weeks. Both PDF views contain the same IDs; Excel weekly counts recalculate to 58. Deliberate bad inputs produced unknown-story, premature-release and missing-dependency errors.
- **Alternative considered and rejected:** Funding and minimum operations cannot wait until the final release if a stay is to be supported. Their necessary stories are therefore explicit R1 dependencies; broader renewal/reporting remains later.
- **Honest limits:** No effort or delivery capacity is validated. Relative weeks and owner roles are proposals; all cards start in Backlog. R1 at Week 6 is a controlled test, R2 at Week 9 a mid-sprint milestone, and R3 at Week 12 remains gated.
- **Revisions:**
  - October 29 2026: followed the supplied release-by-epic layout and added the required weekly view, dependencies, priorities and acceptance criteria.

### Tool 5.4
- **Name:** Customer Journey Workflow and walkthrough
- **Job:** Describe the path from a possible night through approval, stay evaluation and purchaser renewal, including exceptions.
- **Architecture choice:** A 32-step source table, self-contained HTML workflow player and swim-lane view, plus a structural consistency checker. It is a workflow, not a screen prototype.
- **Input:** Canonical journey, happy path, final story IDs, MVC Controllers/Models and release plan; corrected customer-journey-workflow v2.
- **Output:** Journey_Walkthrough_ResisXV.html; Journey_Workflow_ResisXV.xlsx/.md/.json; reusable checker and reports. Five actor lanes: worker, purchaser, product front stage, product back stage and operations/support.
- **Human checkpoint:** Review real approval authority, provider handoffs, response timing and liability. Keep personal context steps labelled no product yet. Do not treat a hypothetical journey as observed behavior.
- **Success criteria:** All six stages have at least two steps and a Controller-linked step. Structural checks passed for 32 steps, 17 decisions and seven failure steps. Negative input caught an unknown Controller and broken target. A Node VM checked script execution and routing to decision/recovery destinations.
- **Alternative considered and rejected:** A straight happy-path diagram was insufficient because it would hide the purchaser and failures. The seven-stage proposal was not treated as accepted; the six existing labels were retained for cross-file consistency.
- **Honest limits:** Full browser rendering and print pagination were not verified because local Chromium was unavailable. Release highlighting is not a transaction simulator. R2/R3 behavior must not be mistaken for delivered R1 functionality.
- **Revisions:**
  - October 29 2026: made funding, provider confirmation, denial, cancellation, arrival problems and renewal explicit; delivered HTML and Excel as the course skill specifies.

### Tool 5.5
- **Name:** Final MRD synthesis and alternatives challenge
- **Job:** Combine the project evidence into a concise decision argument with an explicit next research gate.
- **Architecture choice:** Evidence-led document synthesis, official provider/employment source checks, a Word render/review loop and linked story-board exports.
- **Input:** Four supplied interview-summary records, O01-O40/T1-T5, prior MRD, student budget corrections, motel/hostel comparison request, final journey, MVC and release plan.
- **Output:** ResisXV_Final_MRD_Module5.docx, MRD_ResisXV_Module5.md and final story files. The Word document includes the research limits, hypothesis scoreboard, scenarios, alternatives, market scenarios, risk gates and story appendix.
- **Human checkpoint:** Resolve interview dates/relationships and I4 identity; verify matched provider quotes and buyer authority. Student review is still needed before submission.
- **Success criteria:** Rendered and visually reviewed the Word document. The revision gives motels/hostels their strengths and a falsifiable comparison instead of claiming no alternatives. The account contrast between I1 and I3 changes household-fit segmentation.
- **Alternative considered and rejected:** Unsupported absolute superiority was replaced with comparison against real provider arrangements and returning home. A large workforce is not treated as validated lodging demand or a timely market trend.
- **Honest limits:** The 4.9 million employed CDMX-resident baseline is only a sourced geographic proxy; it excludes cross-border workers such as I1. Qualification, nights, price and reach are scenario assumptions. Public listings are not actual selected-date overnight quotes. There is no funded pilot, completed stay or new interview.
- **Revisions:**
  - October 29 2026: integrated the student’s motel/hostel direction consistently, added scoped TAM/SAM/SOM arithmetic and retained Conditional Go for testing but No Go for paid operation until gates pass.

### Tool 5.6
- **Name:** Final key wireframes and usability plan
- **Job:** Make the registered core path, purchaser decisions and recovery states concrete for design review.
- **Architecture choice:** Twelve grayscale SVG screens, annotated HTML/Markdown, a PDF export, screen checker and reusable review/findings template.
- **Input:** Final 28-story board, MVC, canonical journey, eleven-type content model and explicit M03 accommodation-type addition, earlier eleven-screen drafts and student request to update the key design.
- **Output:** ResisXV_Final_Wireframes_Module5.pdf; linked HTML; twelve editable SVGs; Screen_Flow_ResisXV_Module5.md; usability plan; reusable review template and checker.
- **Human checkpoint:** Review pending versus confirmed support, demo-state navigation, affordability, cancellation terms, provider access and reconciliation. Obtain worker and purchaser feedback before coding a live service.
- **Success criteria:** Twelve key screens map to known R1 stories and fields, with next/back/exit actions. Navigation targets resolve. Structural baseline passed; negative control detected an unknown story, a missing exit and a broken destination. Thirteen PDF pages were rendered and visually checked.
- **Alternative considered and rejected:** A polished mockup or mixing all future features into R1 would obscure scope. Grayscale key screens keep R2/R3 details in annotations; a full operations administration console remains outside this draft.
- **Honest limits:** Prices and approval/ledger states are fictional demo data. Static links do not reserve, approve, settle or test usability. F09 groups exception variants; a runtime version should show only the relevant state. No five-worker or two-approver study has occurred.
- **Revisions:**
  - October 29 2026: added employer setup, request approval and reconciliation; preserved company-wide budget arithmetic and the unaffordable-self-pay block.

### Tool 5.7
- **Name:** Decision logging and cumulative Module 5 handoff
- **Job:** Record what was produced, why it changed and what remains untested without rewriting earlier module history.
- **Architecture choice:** A running Markdown record and deterministic PDF print view assembled from the session, decision log and exported check reports.
- **Input:** Recorded Modules 3 and 4, Module 5 artifacts, student requests/corrections and actual consistency-check results.
- **Output:** DESIGN_DOC_ResisXV_Module5.md and ResisXV_Module5_Design_Document.pdf; current decision log and an organized submission bundle.
- **Human checkpoint:** Review the concrete submission files. The student must upload to Canvas and replace the old context document. Modules 1-2 remain unrecorded; Modules 6-9 are future placeholders.
- **Success criteria:** Module 3 and Module 4 sections remain byte-for-byte unchanged. Module 5 fills all nine tool fields plus dated revisions. The PDF contains the recorded entries; unknown research, approvals and tests remain identified rather than filled with invented results.
- **Alternative considered and rejected:** Recreating a new isolated design record or filling future modules would lose the running history. This update preserves dated snapshots and records current-state changes in Module 5.
- **Honest limits:** The record does not claim Canvas submission, a project-context replacement, permanent skill installation, Trello synchronization or a deployment. This documents drafting effort, not proof of business validation.
- **Revisions:**
  - October 29 2026: added seven Module 5 workflows, actual checks, scope decisions, unresolved research and the final student upload handoff.

### Assignment files and handoff

| Item | Main files | Status |
|---|---|---|
| 1 MVC 1 pager | ResisXV_MVC_One_Pager.pdf | One-page draft, story linked; architecture choices proposed. |
| 2 Final MRD and User Story Board | ResisXV_Final_MRD_Module5.docx; User_Story_Board_ResisXV_Module5.xlsx | Includes 20 worker, 5 purchaser and 3 internal stories; evidence limits and open gates disclosed. |
| 3 Final Design | ResisXV_Final_Wireframes_Module5.pdf | 12 key screens plus IA page; editable SVG/HTML and test plan included. |
| 4 Customer Journey Workflow | Journey_Walkthrough_ResisXV.html; Journey_Workflow_ResisXV.xlsx | Branching workflow and detailed table prepared; browser print layout still unverified. |
| Required planning exercise | ResisXV_12_Week_Scrum_Board.pdf; Scrum_Board_ResisXV.xlsx | 58 cards, six sprints, three release milestones; staffing and calendar unconfirmed. |
| 5 Running design record | DESIGN_DOC_ResisXV_Module5.md; ResisXV_Module5_Design_Document.pdf | Current module recorded; earlier modules preserved. Student uploads PDF and replaces context Markdown. |

### Checks performed and their practical limits

The Scrum linter rejected a nonexistent story, a premature release story and a missing dependency. The journey checker rejected a nonexistent Controller and an invalid target. The wireframe checker rejected an unknown story and a missing or broken exit. The final story checks confirmed four-part wording, 28 IDs and at least two worker stories per canonical stage. These are structural checks, not evidence of research authenticity, usability, capacity or live feasibility.

One rendering limitation remains explicit: the customer workflow’s full browser appearance and one-page print layout were not verified because Chromium was unavailable. A minimal-DOM Node VM exercised script execution and routing after an escaping defect was corrected. This is narrower than a real-browser test. The final Word MRD and wireframe PDF were rendered and visually inspected, and spreadsheet previews were reviewed.

Cross-module limitations remain: the older affinity map still uses provisional stage labels, complete operations-field capture has not been reviewed, and the full operations console is not part of the twelve key screens. Later story and journey releases remain proposed. These open items are not erased by successful ID checks.

### Student contribution and revision reasoning

The student supplied the corrected course skills and two visual examples, asked that the documents match them accurately, requested motel/hostel alternatives, and authorized each next deliverable. Earlier student corrections to funding scope, I4’s budget and excluded-worker effects remained active. The user also clarified that the workflow submission should include HTML and Excel; the response followed the course skill’s deliverable list.

The design keeps purchaser and worker roles separate. Essential support setup, approval, reconciliation and operations move into R1 prerequisites even though broader purchaser/platform features are later. This is an explicit proposed scope change, not a quiet reclassification of evidence. Native apps and automated provider/payment integrations are deferred because no current core story requires them. These rationales are recorded from the drafting process; they do not invent an earlier student debate.

### Remaining work and final submission actions

- Review the final documents and correct missing participant dates, recruitment relationships and I4 identity before presenting the research as fully documented.
- Obtain actual comparable overnight quotes, purchaser authority, rules, worker consent and named operating owners before a live pilot. Public provider listings and hypothetical TAM/SAM/SOM inputs are not those commitments.
- Run the proposed usability study and record observed findings rather than thresholds as results. Verify the workflow in a browser and check its print view.
- Upload the deliverables and the Module 5 design PDF to Canvas. Replace the old running design-document copy in project context with DESIGN_DOC_ResisXV_Module5.md. This session does not perform those external uploads.
- Modules 1 and 2 remain unrecorded because their records were not available. Modules 6-9 remain placeholders for later work.

### Reusable tools retained

Scrum_Card_Linter_ResisXV.py, Journey_Consistency_Check_ResisXV.py, Wireframe_Consistency_Check_ResisXV_Module5.py and Wireframe_Review_Template_ResisXV_Module5.md are included in the handoff. The checker packages retain their input data and recorded negative-control results so their actual scope can be reviewed. The decision log records dated changes without replacing the MRD with a transcript.

---

## Module 6: Positioning, Go-to-Market and PRD

**Status:** recorded to date; assignment work remains open.
**Session date:** November 12, 2026.
**Summary:** I prepared the ResisXV PRD, positioning statement and GTM checklist using the Module 5 research and design work. I asked for the PRD to follow the supplied InstaVacay example, reuse the generated persona image and stay close to my original goals, procedures and roadmap. The completed drafting is recorded below. The Innovation Framework exercise, the required three-example PRD scorecard and second iteration, and the requested original-plan correction are not recorded as complete.

### Goals and source boundaries

The current requirements describe an occasional employer-supported stay near work, with an accepted personal cost, confirmed accommodation and a review of actual rest and expense. Sebastián remains the primary research persona; the authorized employer buyer is a separate role. I2 is not established as Sebastián’s employer, and the shared funding range is not a per-worker allowance.

The PRD carries forward a proposed twelve-week plan with R1 at Week 6, R2 at Week 9 and R3 at Week 12. These are the currently documented milestones, not proof that they match the earlier plan I subsequently asked to restore. The two later Word uploads contain identical extracted paragraph/table text. The original reference I called “PIOGI” has not been identified, so its goals, protocols and roadmap cannot be reconstructed reliably.

### Tool 6.1
- **Name:** PRD synthesis and illustrated requirements document.
- **Job:** Turn the research, stories, workflow and screens into requirements that a product team can review.
- **Architecture choice:** Source-led synthesis into Markdown, editable Word and a rendered PDF. The supplied InstaVacay PRD guides structure and narrative; it is not evidence of ResisXV demand.
- **Input:** Module 5 MRD, 28-story board, MVC, twelve-week Scrum plan, customer workflow, twelve wireframes and original generated persona illustration; supplied InstaVacay example.
- **Output:** PRD_ResisXV.md, PRD_ResisXV.docx and PRD_ResisXV.pdf, plus a source package. The generated PDF has 25 pages, six illustrated use cases, twelve screen references and ten proposed R1 features.
- **Human checkpoint:** Confirm business scope, buyer authority, commercial assumptions and operating responsibilities. Check the original-plan reference before accepting the requested correction as finished.
- **Success criteria:** The drafting pass checked the twelve screen IDs and ten feature IDs, reviewed all rendered PDF pages and checked cost arithmetic. The source distinguishes interview accounts, demo screens and proposed thresholds. These checks do not validate demand or a live implementation.
- **Alternative considered and rejected:** A screen-by-screen tour without tasks would not explain how an accepted stay is funded and completed. The document instead narrates worker, employer and operations steps around specific tasks. Future releases remain higher level than R1.
- **Honest limits:** Funding, provider supply, actual rest gain, pricing and staffing are unverified. The engineering rates and coordination fee are planning assumptions. No booking backend was deployed. The full three-example assignment evaluation was not completed by the internal drafting review.
- **Revisions:**
  - November 12, 2026: produced the 25-page PRD following the example; retained the updated research persona and identified the reused portrait as an illustration.
  - November 12, 2026: corrected the proposed shared-budget logic to include both lodging subsidy and employer-paid coordination fee. The older demo screens do not fully display this addition; the PRD discloses the difference.

### Tool 6.2
- **Name:** Positioning and messaging framework.
- **Job:** Express the intended offer consistently for the worker and employer buyer.
- **Architecture choice:** An eight-section Markdown framework linking the Golden Circle, Moore statement, desired perceptions, three job scenarios, pillars, tagline and source trace.
- **Input:** Final MRD, PRD, primary/secondary persona constraints and six-stage journey. No new interview or message test was added.
- **Output:** Positioning_ResisXV.md. It contains a 43-word Moore statement matching the PRD, three scenarios and the pillars Recover Time, Clear Support and Choose Freely. Working tagline: “One night near work, with employer support.”
- **Human checkpoint:** Review the wording with workers and an authorized buyer. The working tagline is recommended copy, not a recorded user selection or tested message.
- **Success criteria:** The recorded checks confirmed eight required sections, a Moore statement under 50 words that matches the PRD, three job scenarios, three two-word pillars, a seven-word tagline and no drafting placeholders.
- **Alternative considered and rejected:** Generic claims of an AI advantage, guaranteed savings or an exclusive lodging category lack support. The wording instead identifies occasional stays, clear support and worker choice. The other tagline candidates are retained in the file rather than presented as approved choices.
- **Honest limits:** The proposed segment boundary and benefit remain unvalidated. Direct providers or manual employer coordination could offer a similar service. Draft perceptions and stories are not interview quotes, testimonials or observed bookings.
- **Revisions:**
  - November 12, 2026: completed the framework and carried the PRD Vision forward unchanged, with evidence limits and alternative comparisons.

### Tool 6.3
- **Name:** Go-to-market readiness checklist.
- **Job:** Translate the proposed positioning into acquisition, commercial and operational tasks before a pilot.
- **Architecture choice:** A Markdown plan with four route decisions, eight business questions, a status table, seven workstreams, a claims register and PRD open items.
- **Input:** Positioning_ResisXV.md; PRD pricing, costs, metrics and milestone sections; MRD constraints; customer journey.
- **Output:** GTM_Checklist_ResisXV.md. It contains 27 launch items with status, required owner role, target timing and completion evidence.
- **Human checkpoint:** Confirm actual buyer authority, supplier terms, worker consent, payment responsibility, arrival support and the cost of delivering the service. Owner roles are not confirmed hires.
- **Success criteria:** The recorded checks confirmed eight answered business questions, 27 consistently structured checklist rows and ten classified site claims. The register has three Real entries, zero Measured entries and seven Hypothesis entries; Real means a documented account or artifact exists, not an operating-service outcome.
- **Alternative considered and rejected:** Broad paid consumer advertising would not solve missing employer funding. The proposed route is push, vertical and B2B2C, with direct employer sales and employer-mediated worker access. Paid social and subscription tiers are deferred.
- **Honest limits:** The route is a proposal, not evidence of sponsorship or conversion. The MXN 50 coordination fee and 2.7–5.3 month outreach-only payback are assumptions. Full CAC, LTV, fixed-cost coverage and staffed arrival support remain unresolved. No leads were contacted by this checklist.
- **Revisions:**
  - November 12, 2026: completed the GTM plan and separated documented preparation from open launch commitments; retained the PRD’s relative weeks.

### Tool 6.4
- **Name:** Version comparison and original-plan correction review.
- **Job:** Identify whether the later PRD can be aligned with the original goals, procedures and roadmap without inventing them.
- **Architecture choice:** Read-only paragraph/table extraction and text comparison, combined with the recorded student correction.
- **Input:** PRD_ResisXV(1).docx and PRD_ResisXV(2).docx; the instruction to keep design and profiles, restore the original direction and simplify the roadmap.
- **Output:** Comparison finding: both supplied Word files contain the same extracted narrative/table text despite differing binary file sizes. The requested substantive revision remains pending the original source.
- **Human checkpoint:** Identify or supply the original document called “PIOGI.” Preserve the approved design and profiles; do not treat later proposed thresholds or scope as original decisions.
- **Success criteria:** The actual comparison returned no extracted-text differences between the two Word uploads. This supports a narrow version finding, not a claim that their XML, metadata or visual formatting are identical. No missing original goals were filled from memory.
- **Alternative considered and rejected:** Assuming the file labelled (1) was the original would not be justified by its contents. The source was requested instead of silently changing the project direction.
- **Honest limits:** The original reference is unavailable. A phase/objective/activities/expected-result roadmap table was proposed, but the source-aligned revision has not been delivered. The internal single-example drafting review does not satisfy the assignment’s three-example scorecard and second iteration.
- **Revisions:**
  - November 12, 2026: recorded the student’s correction and the identical-text finding; left the source-dependent revision open.

### Tool 6.5
- **Name:** Cumulative Module 6 design record.
- **Job:** Record completed work, student decisions, actual checks and missing assignment evidence while keeping earlier module history.
- **Architecture choice:** Update the running Markdown record and render a cumulative PDF. Earlier module text is preserved as historical evidence, even when it refers to then-future work.
- **Input:** DESIGN_DOC_ResisXV_Module5.md; the PRD, positioning and GTM artifacts; visible session instructions, version comparison and supplied GitHub presentation note.
- **Output:** DESIGN_DOC_ResisXV_Module6.md and ResisXV_Module6_Design_Document.pdf.
- **Human checkpoint:** Review the record, upload the PDF for the assignment and replace the earlier project-context Markdown with the updated file. This action does not submit files to Canvas.
- **Success criteria:** The update checks that Modules 3, 4 and 5 remain byte-for-byte unchanged, adds five Module 6 entries and preserves unrecorded future modules. The PDF is rendered and checked for readable pagination and complete fields before delivery.
- **Alternative considered and rejected:** A standalone summary would omit the cumulative history. Marking all of Module 6 finished would also erase the unresolved exercise, evaluation and original-plan correction. The record instead states progress and open work separately.
- **Honest limits:** This is a record of drafting and review. It does not establish a live service, paid demand, research validation, completed assignment evaluation or Canvas submission. No new skill installation or production integration is claimed.
- **Revisions:**
  - November 12, 2026: recorded the current Module 6 work and prepared the cumulative handoff requested by the student.

### Assignment status and submission evidence

| Deliverable | Recorded status | Remaining action |
|---|---|---|
| Positioning statement | Prepared in Positioning_ResisXV.md. | Review proposed wording and test the benefit. |
| GTM checklist | Prepared in GTM_Checklist_ResisXV.md. | Resolve open launch commitments; checklist completion is not launch approval. |
| PRD | 25-page PDF, Word and Markdown prepared. | Align with the original plan once identified; complete required comparative evaluation and second iteration. |
| Marketing website | Student supplied PRD_Github.html as context, stating a marketing page is published; plans to submit through GitHub. | Use the functioning site and repository links. This record does not independently audit the deployed page or treat the HTML note as the marketing implementation. |
| Innovation Framework exercise | Not recorded as completed. | Complete the supplied exercise and retain its output. |
| Three-example PRD evaluation | Not recorded as completed. | Review all three required examples, produce a scorecard and use it for the next PRD iteration. |
| Module 6 design record | Prepared by this update. | Student reviews, submits the PDF and replaces the old context Markdown. |

GitHub submission references supplied in the project context:

- Website: https://rogaandres.github.io/ResisXV/
- Repository: https://github.com/ROGAAndres/ResisXV

These identify the submission destinations; this update does not certify current page content or change the repository.

### Student contribution and decisions

I supplied the InstaVacay example and asked for a similar PRD structure and narrative, with the previously generated persona image. I then requested the positioning document and GTM checklist. I specified that the marketing page would be submitted through GitHub and clarified that the uploaded HTML and GTM file were context, not an instruction to publish or edit them.

I later asked to preserve the design and persona development while restoring the original goals, protocols and roadmap. That correction remains active. The exact earlier plan must be identified before the narrative is rewritten. Subsequent portrait generation produced separate illustrative images; no replacement of PRD persona images is recorded as completed or authorized by those image requests alone.

### Checks and their limits

The PRD drafting pass reviewed all 25 rendered pages and checked IDs and arithmetic. Positioning checks confirmed the section structure and identical Moore statement. GTM checks counted the eight questions, 27 launch items and ten claims. The two later Word uploads were compared at extracted paragraph/table level and had no text differences.

These checks establish document consistency only. They do not establish customer demand, funding, suitable rooms, operating capacity, causal rest improvements or successful public deployment. Internal critique against the supplied example is not the separate assignment deliverable requiring three examples, a scorecard and a second iteration.

### Remaining work

- Identify the original-plan reference and revise the PRD’s goals, procedures and roadmap against it. Keep the design/profiles and simplify the roadmap presentation.
- Complete the Innovation Framework workflow and save the actual output. No completed innovation exercise is inferred from the PRD.
- Complete the required three-example evaluation, scorecard and revised PRD. Preserve the reasoning behind the changes.
- Check the marketing submission links and claim accuracy as a separate task; no site change is performed by this record.
- Keep live operation at No Go until authorized funding, acceptable supply, worker consent, agreed liabilities and responsible support exist.
- Review and submit this design-record PDF, then replace the older project-context Markdown with the cumulative Module 6 file.

### Reusable outputs

The PRD source, positioning source trace and GTM claims/checklist tables can be reused for the next revision. They remain source-linked documents rather than autonomous agents. Modules 1–2 and 7–9 remain unrecorded; the record does not fill them from inference.

---

## Module 7: Feature Definitions

**Status:** not recorded
**Session date:**
**Summary:**

*(tool entries added on record)*

---

## Module 8: Roadmap and Metrics

**Status:** not recorded
**Session date:**
**Summary:**

*(tool entries added on record)*

---

## Module 9: Go-to-Market Pitch

**Status:** not recorded
**Session date:**
**Summary:**

*(tool entries added on record)*

---

## Change Log

<!-- Claude appends one line per record command. Never deleted. -->

| Date | Command | What changed |
|---|---|---|
| October 15 2026 | Record for module 3 in design document | Restored the existing three-workflow Module 3 record from the prior project copy; historical text preserved with dated revision additions. |
| October 22 2026 | Fill out the design document for module 4 | Recorded seven Module 4 workflows, the student corrections, English deliverables, actual consistency-check controls, open limits and handoff files. Modules 1-2 and 5-9 remain unrecorded. |
| October 29 2026 | Fill out the design document for module 5 | Recorded seven Module 5 workflows, student direction, sourced MRD update, 28-story board, delivery/workflow/design files, actual check results and open gates. Modules 3-4 preserved; 1-2 and 6-9 remain unrecorded. |
| November 12 2026 | Record Module 6 design work to date | Added PRD, positioning, GTM, version comparison and cumulative-record workflows. Preserved Modules 3–5. Innovation exercise, three-example evaluation/second iteration and original-plan correction remain open. |

---

## End-of-semester: Toolkit Summary

*(complete after Module 9: a 250-word index of every tool built, which ones you would keep using on a new idea, and which ones were specific to this venture and would not transfer)*
