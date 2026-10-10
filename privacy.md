---
layout: default
title: ModWatch privacy policy
---

# ModWatch privacy policy

Public product name: **ModWatch**. Approved operator identity: **Victor Bello**. Hosted draft: https://azvicbello-cmd.github.io/modwatch-policies/privacy.html. Effective date: **pending operational verification**.

Pre-release draft awaiting operational verification. Not effective yet. The user confirmed Victor Bello as the final approved operator identity. The user's GitHub account will host the separate `modwatch-policies` repository; it need not belong to the production Reddit account owner. A dated, approved copy is required before release. This draft describes the proposed privacy update, not private version `0.0.1.152`. Policies are prepared for GitHub Pages; if hosted there, page requests are also processed by GitHub under its policies. This does not give the ModWatch app an external data connection.

## Data and purpose

ModWatch reads community rules, removal reasons, and post/user flair templates to provide before/after configuration history to current moderators. It stores original baselines, current snapshots, check times, recent change batches, trigger action types, and available trigger times in Reddit's per-installation Redis storage. Configuration text may itself contain personal information; avoid placing unnecessary personal data in it.

ModWatch checks your current Reddit account and moderator membership to authorize access. It does not persist your account ID for that check. The proposed version does not store trigger moderator names or event IDs. Legacy names/IDs are removed on the next successful app storage read or write after upgrading. A failed cleanup is retried on later operations; it is not reported as completed.

ModWatch does not collect posts, comments, individual flair assignments, passwords, payment information, or advertising profiles. No external data service is configured. The operator does not sell app data or use it for advertising or model training. Reddit operates the hosting/storage platform and processes data under its own policies. Support messages are sent through Reddit, not stored in ModWatch's history.

## Access and retention

Interactive access is restricted to current community moderators. Authorized app operators may access operational logs for support; logs include check summaries and errors, which can contain diagnostic details. Do not submit private configuration text in support screenshots.

History retains up to 25, 50 (default), or 100 recent batches across categories, subject to storage limits. This is a count limit, not a time limit. Original baselines and current snapshots remain while installation storage remains available. Disabling monitoring pauses new observations; it does not erase saved configuration. Uninstalling removes installation history/settings according to Reddit's app lifecycle; reinstalling cannot restore them. There is no off-platform app backup configured.

## Requests and concerns

[Contact ModWatch support](https://www.reddit.com/message/compose/?to=Aggravating_Slice533&subject=ModWatch%20Support) to request access assistance, correction, or removal of personal information stored by ModWatch. Identify the affected community and the information or record concerned. For account-specific requests, send from that Reddit account when possible. Never send passwords, identity documents, or unrelated private moderator data.

The operator reviews requests, verifies only what is necessary, and removes affected stored data or coordinates with Reddit where direct access is unavailable. Requests involving personal information embedded in configuration text may require removing the affected saved configuration, including original baselines; the operator will explain the scope and impact. Removing trigger attribution does not remove information embedded in configuration text. Support handling must not require consent from another moderator as a condition of honoring a valid privacy request. The operator will respond within applicable requirements and communicate any necessary clarification.

Contact support for an account-deletion concern as well. ModWatch does not subscribe to account-deletion notifications or automatically detect personal information inside configuration text. Approved policy changes will be reflected in the dated hosted policy and app documentation.
