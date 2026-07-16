## Week 7 — Issue selection

**Issue link:** https://github.com/ascherj/pathreview/issues/71

**Issue title:** Implement a red-teaming test suite for the prompt injection defense #71

**Tier:** [ ] Tier 1  [ ] Tier 2  [*] Tier 3

**Problem summary:**
[In 3–5 sentences, in your own words: what the issue is (not a copy-paste of
the title), what is currently broken or missing, and what a successful fix would accomplish. Naming the part of the codebase it affects is helpful context.]

The issue consists of creating security test automations that run every time a pull request is made to safely catch changes that weaken the safety layer. These test focus on the safety layer and defending against prompt injection through the ingestion of resumes . These tests affects every file that touches the safety layer and runs in the command line automatically. Currently this app includes no automatic test during pull requests that touch the safety layer. The goal is to protect against various different prompt injection techniques and running tests automatically during PRs to keep that security stable.

**Branch name:** [paste branch name here]

**Setup confirmation:** [ ] App runs locally at localhost:5173

**Cohort ledger:** [ ] Issue added to cohort ledger