## Week 7 — Issue selection

**Issue link:** https://github.com/ascherj/pathreview/issues/71

**Issue title:** Implement a red-teaming test suite for the prompt injection defense #71

**Tier:** [ ] Tier 1  [ ] Tier 2  [*] Tier 3

**Selection Notes:**

Currently my degree and focus is cybersecurity and computer science. This issue does seem difficult in relation to the size of the overall project but relatable to projects I have done during my senior year and in topic. These projects include making a vulnerability prediction tool using linear regression and other models to predict the impact the vulnerabilities on a csv of windows exploits. This issue is actually defending against a vulnerability like prompt injection which requires generating tests and searching examples used by malicious actors. Research and understanding the layout of this project are strong skills used by cybersecurity individuals every day.


**Problem summary:**
[In 3–5 sentences, in your own words: what the issue is (not a copy-paste of
the title), what is currently broken or missing, and what a successful fix would accomplish. Naming the part of the codebase it affects is helpful context.]

The issue consists of creating security test automations that run every time a pull request is made to safely catch changes that weaken the safety layer. These test focus on the safety layer and defending against prompt injection through the ingestion of resumes. These tests affect every file that touches the safety layer and runs in the command line automatically. Currently this app includes no automatic test during pull requests that touch the safety layer. The goal is to protect against various different prompt injection techniques and running tests automatically during PRs to keep that security stable.

**Branch name:** https://github.com/Dannypxp/pathreview/tree/feat/71-red-teaming-suite

**Setup confirmation:** [*] App runs locally at localhost:5173

**Cohort ledger:** [*] Issue added to cohort ledger




## Week 8 — Reproduction & solution planning

**Reproduction commit link:** https://github.com/ascherj/pathreview/commit/1d83a53eeb9263a07db006c947146898354e3a6a

**Reproduction summary:**
[1–2 sentences: How did you reproduce the issue? What did you observe?]

To reproduce the issue, I had to go into "tests/security" to see the red-team suite was not created and no test file was found, this means I would have to create the suite from scratch.

**PLAN.md link:** https://github.com/Dannypxp/pathreview/blob/feat/71-red-teaming-suite/PLAN.md

**Walkthrough video (recommended):** (https://www.loom.com/share/df5fa1c88f0a4eb08ecea3ca12424c9a)

**Blockers or open questions:**
[Anything you're still uncertain about going into Week 9, or leave blank]


## Week 9 — Solution building & PR submission

### Check-in 1 (mid-week)

**Current progress:**
[What have you implemented so far? Which sub-tasks from PLAN.md are done?]
So far I have completed three sub tasks which were to research the missing prompt injection tests from prompt_defense.py, created the new prompt_injection payloads and the test_promp_injection.py to run the payloads.

**Next steps:**
[What are you working on for the rest of the week?]
Next steps are to wire the red team suite to the ci to run the tests everytime a pr touches "safety/". Futhermore, I still have to create conditions for the two edge cases which are for submitting a pr that didnt touch "safety/" and for when a pr changes/alters the prompt_injection tests. Lasty I have to make my pr to submit the assignment.
**Blockers:**
[Anything slowing you down? Or leave blank.]
Claude was down aroun d
---

### Check-in 2 (end of week)

**PR link:** [link to your submitted pull request]

**Branch:** [the branch name you worked on, e.g. `fix/123-short-description`]

**What you built:**
[1–3 sentences summarizing what your fix does and how it works]

**Tests added or updated:**
[Which test files did you touch? What do they cover?]

**Self-review confirmation:** [ ] make check passes  [ ] make test-unit passes

**Draft PR feedback received from:** [name or Slack handle, or "none"]