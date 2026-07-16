## Week 7 — Issue selection

**Issue link:** https://github.com/ascherj/pathreview/issues/71

**Issue title:** Implement a red-teaming test suite for the prompt injection defense #71

**Tier:** [ ] Tier 1  [ ] Tier 2  [*] Tier 3

**Selection Notes:**

Currently my degree and focus is cybersecurity and computer science. This issue does seem difficult in relation to the size of the overall project but relatable to projects I have done during my senior year and in topic. These projects include making a vulnerability prediction tool using linear regression and other models to predict the impact the vulnerabillities on a csv of windows exploits. This issue is actually defending against a vulnerability like prompt injection which requires generating tests and searching examples used by malicious actors. Research and understanding the layout of this project are strong skills used by cybersecurity individuals every day.


**Problem summary:**
[In 3–5 sentences, in your own words: what the issue is (not a copy-paste of
the title), what is currently broken or missing, and what a successful fix would accomplish. Naming the part of the codebase it affects is helpful context.]

The issue consists of creating security test automations that run every time a pull request is made to safely catch changes that weaken the safety layer. These test focus on the safety layer and defending against prompt injection through the ingestion of resumes. These tests affect every file that touches the safety layer and runs in the command line automatically. Currently this app includes no automatic test during pull requests that touch the safety layer. The goal is to protect against various different prompt injection techniques and running tests automatically during PRs to keep that security stable.

**Branch name:** https://github.com/Dannypxp/pathreview/tree/feat/71-red-teaming-suite

**Setup confirmation:** [*] App runs locally at localhost:5173

**Cohort ledger:** [*] Issue added to cohort ledger