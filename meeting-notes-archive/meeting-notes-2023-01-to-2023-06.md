# Meetings notes Archive - 2023 January to 2023 June

## June 6, 5:00 PM ~ 6:00 PM PDT

### Attendees

- Sajay Antony
- Feynman Zhou
- Asmit Malakannawar
- Billy Zha
- Shiwei Zhang
- Terry Howe
- Deepesha Burse

### Agenda

- Celebrate [oras-credential-go v0.2.0](https://github.com/oras-project/oras-credentials-go/releases/tag/v0.2.0) release 
- Discuss when should we merge the oras-credential-go into oras-go (Shiwei)
- Review and confirm the [new ORAS documentation directory strcture proposal](https://docs.google.com/document/d/1mWr7a0jAEMCAupp82AwXUtXNVcWLh4SnfMaLm_zS4co/edit) (Deepesha and Feynman)
- Discuss the maintenance of the [ORAS artifact-spec](https://github.com/oras-project)
- Quick triage for the issues and PRs opened in recent two weeks
- Demonstrate Gitpod support: PR [#186](https://github.com/oras-project/oras-www/pull/186) (Asmit)

### Meeting Notes

- oras-credential-go will be merged to oras-go until it has the RC.1 release
- The [ORAS artifact-spec](https://github.com/oras-project) will be archived after the OCI Image Spec v1.1.0 has a stable release. We will remove [ORAS Artifact Reference Types](https://oras.land/docs/CLI/reference_types) from the ORAS documentation

**Actions:**

- [ ] ORAS maintainers to review [new ORAS documentation directory strcture proposal](https://docs.google.com/document/d/1mWr7a0jAEMCAupp82AwXUtXNVcWLh4SnfMaLm_zS4co/edit) and see if any more doc items should be added
- [x] Asmit to investigate if the GitHub Codespaces can be used as the cloud development environment
- [x] Triage for the issues and PRs opened in recent two weeks


## Next meeting: June 6, 5:00 PM ~ 6:00 PM PDT

### Attendees

* Andrew Block 
* Feynman Zhou
* ToddySM
* Billy Zha
* Yi Zha
* Sylvia Lei
* Shiwei Zhang
* Sajay Antony

### Agenda

- [oras v1.1.0](https://github.com/oras-project/oras/milestone/11) will be released on June 30
- [Artifact Explorer Project Brainstorming](https://docs.google.com/document/d/1nSAnzYcc7050jhDoacTmRMw3asdKd2MZG32MK5Cv3dA/edit#)
- LFX mentorship project updates
    - [Design and implement Artifact Explore web portal](https://mentorship.lfx.linuxfoundation.org/project/9749bc0a-04c9-498d-a16c-e66c0930e819)
    - [Refactor the ORAS documentation structure and write new user guides](https://mentorship.lfx.linuxfoundation.org/project/2314fcc1-f09b-4dab-90fb-d0ef092b6c0e)
- ORAS has a Snap package on Ubuntu now and the next step is to add a GitHub actions to upgrade it per new release automatically

### Meeting Notes

- [x] @Feynman to schedule meetings with two mentees to discuss detailed plans for two projects
- [ ] @Feynman to create an issue to for automating Snap package update in ORAS GitHub Actions

## May 23, 5:00 PM ~ 6:00 PM PDT

### Attendees

* Terry Howe
* Deepesha Burse
* Asmit Malakannawar
* ToddySM
* Billy Zha
* Yi Zha
* Yash Raut
* Sylvia Lei


### Agenda
- Request ORAS maintainers to review Asmit's nomination (PR https://github.com/oras-project/oras-www/pull/181)
- Artifact Explorer Project Brainstorming ([issue 158](https://github.com/oras-project/oras-www/issues/158))
- Allow oras command to skip referrer index clean up ([issue 954](https://github.com/oras-project/oras/issues/954))
- ORAS-go v2.2.0 release ETA date
- CNCF Artifacts Initiative
    - First meeting held Friday May 19
        - Recording: https://www.youtube.com/watch?v=IE7VjiJZx3g
        - Notes: https://docs.google.com/document/d/1E7iKPOuyA1jxPe8vDG8aPd8jtnCEbpDpCifXDvDCnA0/
        - Charter: https://docs.google.com/document/d/1w_lo2RZDKeEzQg4DMV-9Tq4ir_znONj_ypJ27CUfMgY/

### Meeting Notes

- We need to reach super-majority of approvals from ORAS maintainers for Asmit's nomination [PR 181](https://github.com/oras-project/oras-www/pull/181)
- To define a contributor ladder guide in the ORAS community repository
- Walked through the initial ideas of the Artifact Explorer project described in the ([issue 158](https://github.com/oras-project/oras-www/issues/158)). Terry asked if we need to create a new repository for this project 
- We agree the proposal of skiping referrer index cleanup described in the ([issue 954](https://github.com/oras-project/oras/issues/954)). Action items are
    - Toddy will consult this behavior suggestion in the OCI community meeting since cleanup is not defined in OCI distribution Spec yet
    - Feynman will define the output and user experience for the new flag `--gc
- Sylvia will create an issue to vote for releasing ORAS-go v2.2.0. We will cut this release from the `main` branch and change the previous milestone
- Suggest reviewing the first CNCF Artifacts Working Group's meeting [information](https://docs.google.com/document/d/1E7iKPOuyA1jxPe8vDG8aPd8jtnCEbpDpCifXDvDCnA0/) 

### Meeting recording

TBD

## May 9, 5:00 PM ~ 6:00 PM PDT

### Attendees
 - Terry Howe
 - Shiwei Zhang
 - Sylvia Lei
 - Yi Zha
 - Feynman Zhow 
 - Andrew Block 
 - Toddy SM 
 - Billy Zha
 - Asmit Malankannawar
 - 

### Agenda

- The PR of [Working Group Proposal](https://github.com/oras-project/community/pull/48) had majority of approval. Shall we merge it and discuss the next step - Feynman
- Support automatic https-to-http handling via `--insecure` - Billy Zha
    - Discussion: https://github.com/oras-project/oras/discussions/943
    - Issue: https://github.com/oras-project/oras/issues/914
    - Doc: https://hackmd.io/7lGl2zRqQMWt413TttyyVw?view
- Project proposals are submitted to CNCF LFX mentorship program - Feynman
    - [#1 Design and implement Artifact Explore web portal based on ORAS](https://github.com/oras-project/oras-www/issues/158)
    - [#2 Refactor the ORAS documentation structure and write new user guides](https://github.com/oras-project/oras-www/issues/65)
- Introduce @vscoch's project  ORAS-CSI (https://github.com/converged-computing/oras-csi) 

### Meeting Notes
- Discussed flags regarding insecure experience in ORAS CLI, below options discussed
  - option 1: keep `--plain-http` and make insecure flag more specific about tls checking, like `--insecure-skip-tls`
  - option 2: remove `--plain-http` and make `--insecure` handles HTTPS-to-HTTP fallback automatically
- Opion 2 introduces breaking changes into CLI so if we are going to introduce it in 1.X release, there are below options
  - option 2.1: keep `--plain-http`, make flag `--insecure`  covers both HTTP and HTTPS cases with auto fallback (this also introduces breaking change)
  - option 2.2: make no change to existing flags, add a new flag `--insecure-registry` which covers both HTTP and HTTPS cases with auto fallback (this is not optimal since extra flags are introduced)
  - option 2.3: wait for 2.0 release to remove `--plain-http` and make `--insecure` handles both HTTP and HTTPS cases with auto fallback
- Andrew mentioned HELM is going to support HTTP OCI registry by **adding a new flag** to specify plain HTTP
- 
## Apr 25, 5:00 PM ~ 6:00 PM PDT

This meeting was skipped due to no agenda

## Apr 11 2023, 5:00 PM ~ 6:00 PM PDT

### Attendees
 - Feynman Zhou
 - Asmit Malakannawar
 - Alex Flom
 - Shiwei Zhang 
 - Billy Zha
 - Andrew Block
 - Sylvia Lei
 - Steve Lasker
 - Yi Zha
 - Sajay Antony
 - 
### Agenda

- Migrate the new ORAS website implementation to the `dev` branch of oras-www [#PR 140](https://github.com/oras-project/oras-www/pull/140) - Feynman
- Confirm the Working Group setup process and its differences from sub-project https://github.com/oras-project/community/pull/48 - Feynman
- CLI UX issues - Feynman
- Update the [CNCF maintainer list](https://github.com/cncf/foundation/blob/main/project-maintainers.csv#L954) and check the access of https://lists.cncf.io/g/cncf-oras-maintainers
- Setup CNCF/Gitvote for ORAS [@sajay]
    - Draft PR https://github.com/oras-project/community/pull/49


### Meeting notes

We have some actionable items from this meeting:

- [x] ORAS org maintainers to review two PRs https://github.com/oras-project/community/pull/49 and https://github.com/oras-project/oras-www/pull/140
- [x] Terry will submit a PR to update the CNCF maintainer list
- [x] @shizh will help set the Netlify preview for ORAS-WWW dev branch
- [x] Asmit will submit an issue to track the oras go module redirect configuration: https://github.com/oras-project/oras-www/issues/141
- [x] Feynman to continue to clarify the differences between Working Group and sub-project in this PR: https://github.com/oras-project/community/pull/48
- [ ] All ORAS maintainers should join the CNCF mailing group: https://lists.cncf.io/g/cncf-oras-maintainers

## Mar 28 2023, 5:00 PM ~ 6:00 PM PDT

### Attendees
- Feynman Zhou (Microsoft)
- Andrew Block (Red Hat)
- Shiwei Zhang (Microsoft)
- Billy Zha (Microsoft)
- Sylvia Lei (Microsoft)
- Terry Howe (AWS)
- Yi Zha (Microsoft)
- Toddy Mladenov (Microsoft)
- Sajay Antony (Microsoft)
- Asmit Malakannawar (Individual)
- Aaron Friel (Pulumi)
- Alex Flom (Red Hat)

### Agenda

- Configure ORAS Go module name redirects, see [context](https://cloud-native.slack.com/archives/CJ1KHJM5Z/p1679463144003729) (Feynman)
- ORAS installation updates (Feynman)
    - ORAS GitHub Actions has released v1.0.0 and published on the [GH marketplace](https://github.com/marketplace/actions/setup-oras)
    - Added ORAS to NixOS: https://oras.land/cli/#nix
- New ORAS website updates, [preview](https://orasland.netlify.app/) (Asmit)
- Define the charter and scope for the ORAS project 
- New issue triage and PR review
- ORAS governance issues follow-up

### Meeting Notes

- Feynman to create a new issue to list the solutions of configuring ORAS Go module name redirects
- Aaron suggests considering `go install` instructions as another option for installing from latest and opened an issue: https://github.com/oras-project/oras-www/issues/137
- Toddy suggests considering integrating ORAS with other CI/CD systems. Feynman will create issues for this idea and mark them as good-first issues
- Asmit submitted an issue to request to push the new website code to a new branch of ORAS-www: https://github.com/oras-project/oras-www/issues/138
- Feynman will create an issue to open discussion for ORAS project chapter and scope
- Andrew will follow up with CNCF TAG for App Delivery
- Finalize the PR of adding definitation and process for Working Group https://github.com/oras-project/community/pull/48

## Mar 14 2023, 4:00 PM ~ 5:00 PM PDT

### Attendees
- Feynman Zhou (Microsoft)
- Andrew Block (Red Hat)
- Shiwei Zhang (Microsoft)
- Billy Zha (Microsoft)
- Sylvia Lei (Microsoft)
- Terry Howe (AWS)
- Steve Lasker (Individual)
- Yi Zha (Microsoft)
- Toddy Mladenov (Microsoft)
- Sajay Antony (Microsoft)
- Samson Amaugo (Individual)

### Agenda

- Welcome new onwers and thanks Emeritus owners
- [Proposal: Create a new oras-dotnet repository](https://github.com/oras-project/community/issues/38) (Shiwei)
- Refresh oras governance (Toddy)
    - [Clarify the process of setting up a new working group under ORAS
](https://github.com/oras-project/community/issues/33) 
    - [Enforce branch policies on the repository](https://github.com/oras-project/community/issues/41)
- Prepare for the release of [ORAS CLI v1.0.0](https://github.com/oras-project/oras/milestone/15) (Feynman)


## Meeting notes
- Welcomed new project owners.
- Called for review on [oras dotnet SDK sub-project proposal](https://github.com/oras-project/community/issues/38):
  - Feynman will follow up on revising the voting part in [project governance guide](https://github.com/oras-project/community/blob/main/governance/GOVERNANCE.md) but it won't block the new SDK project creation.
  - Shiwei will clarify who will be the owners for the SDK project.
  - The SDK's Github repository will start  as private and become public once the issue is resolved.
- Discussed on the Github issue: [creating a new oras working group](https://github.com/oras-project/community/issues/33), called for commenting.


## Feb 28 2023, 4:00 PM ~ 5:00 PM PST

### Attendees

- Alex Flom (Red Hat)
- Lachlan Evenson (Microsoft)
- Feynman Zhou (Microsoft)
- Gavin Scallon (Individual)
- Andrew Block (Red Hat)
- Shiwei Zhang (Microsoft)
- Terry Howe (AWS)
- Steve Lasker (Individual)
- Ramkumar Chinchani (Zot)
- Yi Zha (Microsoft)
- Sajay Antony (Microsoft)
- Asmit Malakannawar (LFX mentee)
- Toddy (Microsoft)

### Agenda

- Introduce [OCI Search API Working Group Vision](https://docs.google.com/document/d/1rcQROZP31q7BOjoZ977Ok7pt28z_UXfW0vAK3xC0wdI/edit?usp=sharing) (Toddy)
- [Disable auto conversion of manifest types](https://github.com/oras-project/oras/issues/782) proposed by Sajay
- Discuss and confirm a regular release cadence for ORAS-go v2 and deprecation plan of ORAS-go v1 (Feynman)
- Review the status of new issues, PRs, and proposals
- Add Billy Zha's GPG Key to `oras` for future releases (Shiwei)
    - PR: https://github.com/oras-project/oras/pull/844
- Josh submitted an [issue](https://github.com/oras-project/community/issues/32) to request step down (org owner and sub projects)

### Meeting notes

- Welcome Gavin to the community
- Discussed and agreed to disable auto conversion of manifest type, and change the default to image manifest
- Per Josh's intent to step down, need a PR to move Josh from org-level owners to emeritus
- Create an issue and PR to nominate Andrew as ORAS org maintainter
- Andrew introduced OCI search API WG vision. The next step is to update the governace document for setting up new subproject and WG, and adding maintainers accordly.
- Toddy will create issues to request updating the governance
- Ask for PR review on adding Billy's GPG key for release purpose
- Feynman will raise an issue to discuss and confirm a regular release cadence for ORAS-go v2 and deprecation plan of ORAS-go v1

## Next meeting: Feb 14 2023, 4:00 PM ~ 5:00 PM PST

### Attendees

* Sylvia Lei
* Billy Zha
* Terry Howe
* Yi Zha
* Feynman Zhou
* Alex Flom
* Gavin Scallon
* Shiwei Zhang
* Asmit Malakannawar

### Agenda

- Introduce [CNCF LFX Mentoring program 2023](https://github.com/cncf/mentoring/tree/main/lfx-mentorship/2023/01-Mar-May) and ORAS proposals
- Refresh community governance guide and process, see [proposal issue](https://github.com/oras-project/community/issues/28) (Feynman)
- Nominate Terry and Billy to be subporect maintainers for ORAS (Feynman)
- Talk about one or more of the following (Terry)
    - https://github.com/oras-project/oras/issues/730 (upload/download)
    - https://github.com/oras-project/oras/issues/799 (tags list filter)
    - https://github.com/oras-project/oras/issues/806 (get tag digest)
    - https://github.com/oras-project/oras/issues/807 (expose cmd level in go)
- General discussion on ORAS Website (Bhawna )
  - Discussion on the figma file of new ORAS Website. It would be helpful to write the proposol in more details.
  - What type of candidate you are looking for completing this project. Like hugo expert and somewhat like that.
  - How many candidate you are looking to select in this March term.
- Talk about one or more of the following (Amisha)
    * Initial discussion regarding the ORAS contribution
    * https://github.com/oras-project/oras-www/pull/103
    * https://github.com/oras-project/oras-www/issues/113    
- Introduce the initial proposal to the new ORAS website (Asmit Malakannawar)
- [Disable auto conversion of manifest types](https://github.com/oras-project/oras/issues/782) proposed by Sajay

### Meeting notes

- Shiwei will create PRs to nominate Terry and Billy to be subporect maintainers for ORAS 
- Submission of the [CNCF LFX Mentoring program 2023](https://github.com/cncf/mentoring/tree/main/lfx-mentorship/2023/01-Mar-May) will be closed on Feb 21
- Asmit Malakannawar shared his thoughts on the ORAS website proposal and prototype design
- 

## Jan 31, 2023, 4:00 PM ~ 5:00 PM PST

### Attendees

- Yi Zha (Microsoft)
- Aaron Friel (Pulumi)
- Sajay Antony (Microsoft)
- Shiwei Zhang (Microsoft)
- Andrew Block (Red Hat)
- Sylvia Lei (Microsoft)
- Jennifer Power (Red Hat)
- Alex Flom (Red Hat)
- Ramkumar Chinchani (Cisco/Zot)
- Steve Lasker (Individual)


### Agenda
- WG for search API https://github.com/oras-project/artifacts-spec/issues/72 (from Toddy Mladenov)
- Archive the artifact-spec repository https://github.com/oras-project/artifacts-spec/pull/119 (from Toddy Mladenov as per Michael Brown's PR)
- Release ORAS CLI v1.0.0 RC.1 (from Feynman)
- [Proposal: SDK for oras login](https://github.com/oras-project/oras-go/discussions/413) (from Shiwei)

### Meeting Notes
- Round table introduction, and welcome new participant Jennifer Power.
- The way forward for search API WG was discussed, and it is agreed during the meeting that is We establish the working group under oras-project first, and inform OCI once we have done some initial work. Other parties in the OCI group will be invited to share theirs work or insights.
- Proposal of SDK for oras login was discussed, and we agreed on the proposal during the meting. Shiwei will create a new repo and create an issue for governance guidance support
- The governace documents need to be updated for creating new repos and adding/updating maintainers for the repos. We could file an issue under oras-project/community repo to address these issues.
- Feynman did a brief intro on oras cli v1.0.0-rc.1 release.
- Regarding to agenda item "archive the artifact-spec repository", it is suggested to hold on the archive until things becomes clear on the OCI artifact manifest direction. A FAQ document is required to help the users understand the way forward for oras/artifact-spec, which also depends on how OCI artifact manifest issue is resolved.
- ORAS community meeting has changed from once a week to bi-weekly

## Jan 10, 2023, 4:00 PM ~ 5:00 PM PST

### Attendees

- Andrew Block (Red Hat)
- Alex Flom (Red Hat)
- Billy Zha (Microsoft)
- Feynman Zhou (Microsoft)
- Shiwei Zhang (Microsoft)
- Sylvia Lei (Microsoft)
- Nima Talebi (Amazon)
- Yi Zha (Microsoft)
- Terry Howe (Amazon)

### Agenda
- New year blog for ORAS
- [Proposal for adding compatibility mode](https://github.com/oras-project/oras/pull/739) 
- Demo for OCI image layout by Billy
- Walk through new feature requests to ORAS
    - [oras cp fails when copying artifacts to an OCI 1.0 registry](https://github.com/oras-project/oras/issues/727) by Aaron
    - [oras repo ls to support sub namespaces](https://github.com/oras-project/oras/issues/733) by Steve
    - [Add ability to download/upload one or more resources to/from disk](https://github.com/oras-project/oras/issues/730) by Terry
- ORAS v1.0.0-RC.1 and ORAS-go v2.0.0 status sharing: 
    - ORAS CLI v1.0.0-rc.1: before Jan 18, 2023
    - ORAS-go v2.0.0: within Jan, 2023
- Request to [add GitHub Actions for ORAS](https://github.com/oras-project/oras/issues/744)

### Meeting notes

- Billy will prepare for the OCI layout doc to include the prototype binary download steps
- Terry asked a question: when using different folders or tar files to store the downloaded artifacts, will the blobs be shared across oci-layout without duplication? The answer is no by default in oci-layout spec, but community suggests that it's possible to hack the sharing, like hard-link `blobs` folders to a centralized folder.
- Triage the feature requests [oras cp fails when copying artifacts to an OCI 1.0 registry](https://github.com/oras-project/oras/issues/727) and [oras repo ls to support sub namespaces](https://github.com/oras-project/oras/issues/733)
- Publish the ORAS new year blog on Jan 11
- Created a good-first issue to [add GitHub Actions for ORAS](https://github.com/oras-project/oras/issues/744)

