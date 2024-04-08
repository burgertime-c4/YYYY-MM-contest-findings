# [Sponsorname] Audit

Audit findings are submitted to this repo.

Unless otherwise discussed, this repo will be made public after audit completion, sponsor review, judging, and issue mitigation window.

**Contributors to this repo:** prior to report publication, please review the [Agreements & Disclosures](/issues/1) issue.

---

# Review phase 

Sponsors have three critical tasks in the audit process:

1. [Respond to issues ↓](#1-respond-to-issues)
2. [Weigh in on severity ↓](#2-weigh-in-on-severity))
3. [Share your mitigation of findings ↓](#3-share-your-mitigation-of-findings)

<hr>
  <details>
  <summary>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<h2>Types of findings</h2> (expand to read more)</summary>

### High or Medium risk findings
Wardens submit issues without seeing each other's submissions, so keep in mind that there will always be findings that are duplicates. For all issues labeled `3 (High Risk)` or `2 (Medium Risk)`, these have been pre-sorted for you so that there is only one primary issue open per unique finding. All duplicates have been labeled `duplicate`, linked to a primary issue, and closed.


### QA reports, Gas reports, and Analyses

All warden submissions in these three categories are submitted as bulk listings of issues and recommendations:

- **[QA reports](https://docs.code4rena.com/roles/wardens/judging-criteria#qa-reports-low-non-critical)** include *all* low severity and non-critical findings from an individual warden.
- **[Gas reports](https://docs.code4rena.com/roles/wardens/judging-criteria#gas-reports)** include *all* gas optimization recommendations from an individual warden.
- **[Analyses](https://docs.code4rena.com/roles/sponsors#analysis-pool)** contain high-level advice and review of the code: the "forest" to individual findings' "trees.”
</details>
<hr>

## 1. Respond to issues

### [Findings for review →](../../issues?q=is%3Aopen+label%3Abug+is%3Aissue+-label%3Aunsatisfactory+-label%3A%22insufficient+quality+report%22+-label%3A%22sponsor+acknowledged%22+-label%3A%22sponsor+confirmed%22+-label%3A%22sponsor+disputed%22+-label%3A%22judge+review+requested%22+-label%3A%22QA+%28Quality+Assurance%29%22+-label%3A%22G+%28Gas+Optimization%29%22)

For each High or Medium risk finding that appears [in this filtered issues view](../../issues?q=is%3Aopen+label%3Abug+is%3Aissue+-label%3Aunsatisfactory+-label%3A%22insufficient+quality+report%22+-label%3A%22sponsor+acknowledged%22+-label%3A%22sponsor+confirmed%22+-label%3A%22sponsor+disputed%22+-label%3A%22judge+review+requested%22+-label%3A%22QA+%28Quality+Assurance%29%22+-label%3A%22G+%28Gas+Optimization%29%22), please label as one of these:

- `sponsor confirmed`, meaning: "Yes, this is a problem and we intend to fix it."
- `sponsor disputed`, meaning either: "We cannot duplicate this issue" or "We disagree that this is an issue at all."
- `sponsor acknowledged`, meaning: "Yes, technically the issue is correct, but we are not going to resolve it for xyz reasons."

Add any necessary comments explaining your rationale for your evaluation of the issue. 

**Note that when the repo is public, after all issues are mitigated, wardens will read these comments; they may also be included in your C4 audit report.**

## 2. Weigh in on severity 

If you believe a finding is technically correct but disagree with the listed severity, leave a comment indicating your reasoning for the judge to review.
For a detailed breakdown of severity criteria and how to estimate risk, please refer to the [judging criteria in our documentation](https://docs.code4rena.com/awarding/judging-criteria/severity-categorization).

Judges have the ultimate discretion in determining validity and severity of issues, as well as whether/how issues are considered duplicates. However, sponsor input is a significant criterion.

### Once labelling is complete

When you have finished labelling findings, drop the C4 team a note in your private Discord backroom channel and let us know you've completed the sponsor review process. At this point, we will pass the repo over to the judge to review your feedback while you work on mitigations.  

## 3. Share your mitigation of findings

*Note: this section does not need to be completed in order to finalize judging. You can continue work on mitigations while the judge finalizes their decisions and even beyond that. Ultimately we won't publish the final audit report until you give us the OK.*

For each finding you have confirmed, you will want to mitigate the issue before the contest report is made public.

### If you are planning a Code4rena mitigation review:
1. In your own Github repo, create a branch based off of the commit you used for your Code4rena audit, then
2. Create a separate Pull Request for each **High or Medium risk** C4 audit finding (e.g. one PR for finding H-01, another for H-02, etc.)
3. Link the PR to the issue that it resolves within your contest findings repo.

Most C4 mitigation reviews focus exclusively on reviewing mitigations of High and Medium risk findings. Therefore, QA and Gas mitigations should be done in a separate branch. If you want your mitigation review to include QA or Gas-related PRs, please reach out to C4 staff and let’s chat!

If several findings are inextricably related (e.g. two potential exploits of the same underlying issue, etc.), you may create a single PR for the related findings.

### If you aren’t planning a mitigation review

1. Within a repo in your own GitHub organization, create a pull request for each finding.
2. Link the PR to the issue that it resolves within your contest findings repo.

This will allow for complete transparency in showing the work of mitigating the issues found in the contest. If the issue in question has duplicates, please link to your PR from the open/primary issue.
