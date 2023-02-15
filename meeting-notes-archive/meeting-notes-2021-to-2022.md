# An archive of the ORAS Community Meeting Notes from 2021 to 2022 

This document is an archive of notes captured at https://hackmd.io/P-O6n222TcSMoJgHmTTduw?view.

## Dec 12, 2022, 4:00 PM ~ 5:00 PM PST

### Attendees

- Billy Zha
- Feynman Zhou
- Shiwei Zhang
- Sylvia Lei
- Ramkumar Chinchani
- Yi Zha 

### Agenda

- [ORAS-go v2.0.0-RC.6](https://github.com/oras-project/oras-go/releases/tag/v2.0.0-rc.6) release walkthrough
- Upcoming milestone and timeline updates
    - ORAS CLI v1.0.0-rc.1: Jan 9, 2023
    - ORAS-go v2.0.0: Jan 16, 2023
    - ORAS CLI v1.0.0: Feb 6, 2023
- (Potential) Preparation for the [CNCF incubating criteria](https://github.com/cncf/toc/blob/main/process/graduation_criteria.md#incubating-stage)

## Dec 6, 2022, 4:00 PM ~ 5:00 PM PST

Canceled due to no agenda gathered this time

## Nov 29, 2022, 4:00 PM ~ 5:00 PM PST

### Attendees

- Aaron Friel
- Alex Flom
- Billy Zha
- Feynman Zhou
- Shiwei Zhang
- Sylvia Lei
- Ramkumar Chinchani
- Yi Zha

### Agenda

- Ramkumar to introduce Zot and demonstrate how to use ORAS v0.16 to distribute OCI artifacts to Zot registry
- Q & A

## Nov 15, 2022, 4:00 PM ~ 5:00 PM PST

### Attendees

- Feynman Zhou
- Shiwei Zhang
- Sylvia Lei
- Andrew Block
- Sajay Antony
- Nima Talebi
- Billy Zha
- Yi Zha

### Agenda

- Support OCI image layout discussion, see [issue](https://github.com/oras-project/oras/issues/378) and [draft proposal](https://hackmd.io/ogglvwhLTVW2-T6b2JC_Gg?view)
- [ORAS-go v2.0.0-rc.5](https://github.com/oras-project/oras-go/milestone/9) release is planned to be released on Nov 17
- Follow up the actionablt items in the last meeting:
    - Toddy will help to validate the issue of [when coping windows-based images with non-distributable(foreign) layers](https://github.com/oras-project/oras-go/issues/319)
    - Feynman will create a GitHub issue to track the new documentation structure work - Done, see [issue 65](https://github.com/oras-project/oras-www/issues/65) 
    - Sajay will help to confirm the criterial and timeline of cutting a stable release in OCI image-spec
- Q & A

### Meeting notes
- Support OCI image layout
    - CLI UX
        - Vote for two options
            - Use prefixes
            - Use flags
    - Q:Can we use oci-layout for caching?
        - OCI Layout folder is a ORAS Cache folder plus a index file. ORAS Cache (i.e. a file based CAS) can be R/W concurrently. However, OCI layout folder is not. Because, the index file is not concurrent safe. Especially, we have multiple processes accessing the same file system.
    - Q: It would be nice if we can read manifests as well. For e.g. ratify could then use the cache as backing store (This is not in current scope)
- OCI Image & distribution spec stable release will be cut probably next year 2023
## Nov 8, 2022, 4:00 PM ~ 5:00 PM PST

### Attendees

- Feynman Zhou
- Billy Zha
- Sylvia Lei
- Shiwei Zhang
- Toddy
- Yi Zha
- Nima
- Alex Form
- Clark Porter

### Agenda

- Celebrate the ORAS CLI 0.16 release
- [Add ReferrerFinder to Repository interface](https://github.com/oras-project/oras-go/issues/356) - Shiwei

## Nov 1, 2022, 5:00 PM ~ 6:00 PM PST

### Attendees
- Feynman Zhou
- Andrew Block
- Billy Zha
- Sylvia Lei
- Shiwei Zhang
- Lin Cao
- Toddy
- Clark Porter
- Nima 
- Yi Zha
- Sajay

### Agenda
1. Celebrate the ORAS-go v2.0.0-RC.4 release [https://github.com/oras-project/oras-go/releases/tag/v2.0.0-rc.4]
2. [ORAS documentation plan](https://hackmd.io/uXm-q0aDQ96hyB6TIWNh_w?view#New-Documentation-Directory1) walkthrough
3. Short updates on the ORAS Future milestones
4. Since Dockerhub doesn't support the Subject field should the CLI maybe remove subject when image manifest push fails or should we wait for Docker hub to support it? 

### Meeting notes

- Breaking changes for RC4
- Actionablt items:
    - Toddy will help to validate the issue of [when coping windows-based images with non-distributable(foreign) layers](https://github.com/oras-project/oras-go/issues/319)
    - Feynman will create a GitHub issue to track the new documentation structure work
    - Sajay will help to confirm the criterial and timeline of cutting a stable release in OCI image-spec

## Oct 25, 2022, 5:00 PM ~ 6:00 PM PST

Cancelled this occurrence due to no agenda gathered and KubeCon NA this week.


## Oct 18, 2022, 5:00 PM ~ 6:00 PM PST

### Attendees
- Feynman Zhou
- Alex Flom
- Nima 
- Lin Cao
- Shiwei Zhang
- Vishrut Patel
- Andrew Block
- Sajay Antony
- Yi Zha
- Billy Zha
- Sylvia Lei
- Toddy Mladenov
- Nora Hu

### Agenda

- [ORAS-go v1.2.1](https://github.com/oras-project/oras-go/releases/tag/v1.2.1) and [ORAS CLI v0.15.1](https://github.com/oras-project/oras/releases/tag/v0.15.1) released this week
- [Retry design proposal updates](https://github.com/oras-project/oras-go/discussions/232#discussioncomment-3804712)
- Provide [ORAS CLI reference documentation](https://github.com/oras-project/oras-www/issues/59)
- Discuss possibility of shortening the commands like `repository` to just `repo` and other usability improvements @sajay 
- Demo: OCI artifact support in ORAS CLI (Billy)
- Demo: ORAS CLI 0.15 and blog post walkthrough

### Meeting notes

- Review ORAS CLI 0.15 blog post
- Create a GitHub issue to track the request of shortening ORAS CLI command
- Record a demo for OCI artifact support in ORAS CLI

## Oct 11, 2022, 5:00 PM ~ 6:00 PM PST

### Attendees
- Feynman Zhou
- Alex Flom
- Nima 
- Lin Cao
- Shiwei Zhang
- Vishrut Patel
- Andrew Block
- Sajay Antony
- Yi Zha

### Agenda
- ORAS CLI 0.15 live demo
- [ORAS migrating to OCI reference types doc](https://hackmd.io/zLnCh8WRQDG-3S_jXR626g?view) updates
- [Retry design proposal updates](https://github.com/oras-project/oras-go/discussions/232#discussioncomment-3804712)
- Follow up issue [Transfer-Encoding: chunked responses fail](https://github.com/oras-project/oras-go/issues/333) with Nima
- Provide [ORAS CLI reference documentation](https://github.com/oras-project/oras-www/issues/59)
- Discuss possibility of shortening the commands like `repository` to just `repo` and other usability improvements @sajay 

### Meeting notes
 - reorder the ORAS CLI demo to the end and prioritize other items that need discussion - Nima
 - Oras Migration - ORAS Artifacts will be deprecated from v2.0.0-rc.4
     - There is no dual support of ORAS artifact and OCI artifacts. 
     - Discuss fallback/compatibility flag names 
         - Does the CLI provide a choice or is that a portion of the spec. 
         - Why did we chose max,min. 
         - Can we differ the issue of compatability to a future release. 
         - Are there are Terms of Service issues in store non-image like data a Container Registry (Alex)
         - Compatability could be considered as ON/OFF as well - @Nima
         - I was thinking that --always-fallback would be `--no-fallback=false (default)` @Alex
     - Deleting manifest
         - Should we delete from leaf nodes to parent? @sajay 
     - Implement the default spec and create issues to dicuss advanced cases with capability mode @yizha1  

 - Actionable items:
     - Feynman will create a blog to demonstrate the ORAS CLI 0.15 demo
     - Feynman and Yi will create GitHub issues for advanced compatability of `oras push` and `oras attach`
     - Nima follows up the issue of [Transfer-Encoding: chunked responses fail](https://github.com/oras-project/oras-go/issues/333)
    

## Sep 28, 2022, 5:00 PM ~ 6:00 PM PST

### Attendees
 - Feynman Zhou
 - Sajay Antony
 - Yi Zha
 - Lin Cao
 - Nima Talebi
 - Vishrut Patel
 - Billy Zha
 - Shiwei Zhang

### Agenda
- ORAS CLI 0.15 is released, see [Release Notes](https://github.com/oras-project/oras/releases/tag/v0.15.0)
- Share the [ORAS CNCF annual review](https://hackmd.io/sbXNtb56RmSq1JqsgUHNIA?view)
- [Transfer-Encoding: chunked responses fail in ECR with ORAS](https://github.com/oras-project/oras-go/issues/333)
- [Initial plan of ORAS migrating to OCI in ORAS-go](https://github.com/oras-project/oras-go/issues/271)
- [Propose to publish a new release of fixpack for ORAS-go v1](https://github.com/oras-project/oras-go/issues/278)

### Notes 
 - RC2 for image spec is need to get the `refers` field rename as it was missed in the v1.1.0-rc1 release https://github.com/opencontainers/image-spec/pull/958
 - Current implementation for oras-go with OCI support - 
     - https://github.com/oci-playground/oras-go
- Welcome Lin and Vishrut
- Introduced new ORAS CLI release 0.15.0
    - Testing towards GAR is in-process
- Feynman shared ORAS CNCF annual review report
- Issue discussion [Transfer-Encoding: chunked responses fail in ECR with ORAS](https://github.com/oras-project/oras-go/issues/333)
    - ECR respones chunked manifest to the client
    - Considering ORAS to support Chunked manifest for pull request
- ORAS will only support OCI artifact, no fallback to ORAS artifact
- Should we consider pushing the changes directly to main rather than having another branch @sajay 
- ORAS migrating to OCI artifact document will be updated this week
- ORAS supporting OCI artifact in ORAS-go is planned in ORAS v2.0.0-rc.4
- Sajay shared a good practice for cutting a release
- Feynman will upload the recorded meetings into Youtube



## Sep 13, 2022, 5:00 PM ~ 6:00 PM PST

### Attendees
- Sajay Antony
- Feynman Zhou
- Yi Zha
- Nima Talebi
- Andrew Block
- Haoliang Yue
- Shiwei Zhang
- Steve Lasker
- Sylvia Lei

### Agenda

- [ORAS migrating to OCI Reference types](https://hackmd.io/@yizha1/ORAS_to_OCI_reference_type)
- [Migrate to OCI Artifact from ORAS Artifact in ORAS-go](https://github.com/oras-project/oras-go/issues/271) 
- [Propose to publish a new release of fixpack for ORAS-go v1](https://github.com/oras-project/oras-go/issues/278)
- [Write blog series for ORAS CLI with ACR, ECR, GAR](https://github.com/oras-project/oras-www/issues/54)

### Meeting Notes

- [Migrate to OCI Artifact from ORAS Artifact in ORAS-go](https://github.com/oras-project/oras-go/issues/271)  is planned on ORAS-go v2.0.0-rc.4
- a new release of fixpack for ORAS-go can be cut in Sep
- Feynman will drive the issue of [Write blog series for ORAS CLI with ACR, ECR, GAR](https://github.com/oras-project/oras-www/issues/54)

## Sep 6, 2022, 5:00 PM ~ 6:00 PM PST

### Attendees

- Billy Zha
- Nima Talebi
- Feynman Zhou
- Yi Zha
- Sajay Antony
- Shiwei Zhang
- Billy Zha
- Sylvia Lei

### Agenda
- [Released a patch ORAS v0.14.1 to fix ORAS usability issues with AWS ECR and Google GAR](https://github.com/oras-project/oras/releases/tag/v0.14.1)
- [ORAS Feature List and Roadmap](https://hackmd.io/c-q1od6tTlufHbMJC5T4SQ?view) walkthrough and discussion

### Meeting Notes

- Nima Talebi is interested in taking the issue of [Push / Pull Artifacts from OCI Image Layout #378](https://github.com/oras-project/oras/issues/378) and [Support customer-defined http headers#503](https://github.com/oras-project/oras/issues/503)
- Bring the OCI reference types support plan in the next community call

## Aug 30, 2022, 5:00 PM ~ 6:00 PM PST

### Attendees
- Andrew Block
- Alex Flom
- Nima Talebi
- Feynman Zhou
- Yi Zha
- Shiwei Zhang
- Billy Zha
- Sylvia Lei

### Agenda

- ORAS CLI 0.14 was released, see [Release Notes](https://github.com/oras-project/oras/releases/tag/v0.14.0)
- Preview of [ORAS CLI 0.15](https://hackmd.io/aLxws7mhSZukfFzx3PKq3w?view) and ORAS-go 2.0.0-RC.3 
- UOR framework demo and ORAS-go use case
- ORAS will support OCI artifact menifest and provide backward compatability
- Request to upgrade [ORAS-go from v1 to v2](https://github.com/helm/helm/blob/main/go.mod#L45) in Helm

### Meeting notes

- UOR framework demo, by Andrew and Alex
    - https://universalreference.io
    - https://uor-framework.github.io/
- Walk through release notes for ORAS CLI v0.14.0
- ORAS CLI v0.15.0
    - New commands will be supported
- ORAS-go v2.0.0-rc.3
    - New APIs for simplified UX
- Still planning for ORAS supporting OCI artifact, more details will come later
- Andrew will help to bring this request to Helm community to get the conversion going. The expectation is ORAS-go GA release for Helm to uplift.

## Aug 16, 2022, 5:00 PM ~ 6:00 PM PST

### Attendees

- David Tesar
- Feynman Zhou
- Sajay Antony
- Shiwei Zhang
- Sylvia Lei
- Yi Zha
- Haoliang Yue
- Zhuyu(Zoey) Li

### Agenda

- Celebrate the new release: ORAS-go 2.0.0-rc.2
- Prepare for the release of ORAS CLI v0.14.0
- Feature request from Shiwei: [Output the descriptor of pushed artifact by oras push](https://github.com/oras-project/oras/issues/497)
- Discuss `--artifact-type` support in `oras push`: https://github.com/oras-project/oras/issues/466
- ORAS to support OCI artifact spec
- PR review: https://github.com/oras-project/oras-py/pull/42

## Meeting notes

- ORAS CLI v0.14.0 will be released on Aug 19
- Raise a GitHub discussion to dicuss when to support and transition to OCI artifact spec
- Request Billy Zha to help with ORAS-py [PR review](https://github.com/oras-project/oras-py/pull/42)


## Aug 10, 2022, 5:00 PM ~ 6:00 PM PST

### Attendees

- Alex Flom
- Andrew Block
- Billy Zha
- David Tesar
- Feynman Zhou
- Sajay Antony
- Shiwei Zhang
- Steve Lasker
- Sylvia Lei
- Xu Yang
- Zhuyu(Zoey) Li

### Agenda

- Sajay will share some updates about wg-reference-types and key takeaways related to ORAS
- Feynman will give a demo for previewing ORAS 0.14 and call for testing
- Billy will share his proposal to ORAS E2E testing framework
- ORAS user story discussion (Moved to next time)

### Meeting Notes

- Sajay shared the updates about wg-reference-types
    - [Working Group Proposal for Reference Types from Lachie (Microsoft)](https://github.com/opencontainers/image-spec/pull/934/files)
    - [Working Group Proposal for Reference Types from Michael (Amazon)](https://github.com/opencontainers/distribution-spec/pull/335/files)
    - [Add filtering to references API from Michael (Amazon)](https://github.com/oci-playground/distribution-spec/pull/9/files)
- Feynman demonstrated an end-to-end use case of how to use the new features of ORAS 0.14 (oras copy, attach, discover) with MCR, ACR, and Docker SBOM
- Andrew shared his contribution to Helm: [Attach annotations to OCI artifacts](https://github.com/helm/helm/pull/11204)
- Billy shared his [proposal to ORAS E2E testing framework](https://github.com/oras-project/oras/discussions/485) and waiting for suggestions from the community



## July 6, 2022, 5:00 PM ~ 6:00 PM PST

### Attendees

- Sajay Antony
- Steve Lasker 
- Alex Flom
- Andrew Block
- Shiwei Zhang
- David Tesar
- Akash Singhal
- Billy Zha
- Clifford Sutter
- Patric Zheng
- Vanessa Sochat

### Agenda and Notes

- Celebrate the new release: ORAS CLI 0.13.0 and ORAS-go 2.0.0-Alpha
- What’s new in ORAS 0.14.0 and how to build & test it in advance
- ORAS-artifacts-spec GA (proposed by Sajay)
- ORAS-python future work discussion
- Propose to create a GitHub project board for ORAS
- Discuss command UX for [ORAS Copy](https://github.com/oras-project/oras/issues/307)
- Q & A

-- NOTES -- 
    - Possibly add an issue template to provide guidance of adding new capabilities to ORAS. - @Feynman, Vanessa 
    - Consider exposing OCI store for caching scenarios - sajay/Alex.
    - 


### Action items

## January 05, 2022

### Attendees

### Agenda and Notes
- [Scott] ORAS community maturity updates [oras-project/community#9](https://github.com/oras-project/community/issues/9)
- []

### Action items


## November 18, 2021

### Attendees:
- Steve Lasker (Microsoft)
- Sajay Antony (Microsoft)
- Josh Dolsky (Blood Orange)
- Scott Rigby (Weaveworks)
- Tejaswini Duggaraju (Microsoft)

### Agenda Items:
- ORAS `v1.0.0` first stable release
- backwards compatibility contract
- Community managers role
- Various suggestions to help project maturity
    - <https://github.com/oras-project/community/issues/9>

### Notes:
- Yes to backwards compatibility contract 🎉
- Yes to Scott helping, just need to do something official
    - For now Scott will make a PR to add "community managers" role to <https://github.com/oras-project/community/blob/main/governance/RELEASE-PROCESS.md>
    - then can make an issue to add Scott to that role, which maintainers can vote on
    - Scott: i'm happy however as long as we do it correctly :-)
- Plan for oras-go development and release strategy (summary):
    - Create new `v1` branch based on the `v0.5.0` release commit (`293f55c`)
    - Update go modules/dependencies on `v1`
    - Release a `v1.0.0` release based on the `v1` branch
    - `v1` branch will be maintained primarily for stability/security updates, with Helm as primary customer
        - If possible we can port tag listing work from `main` into a `v1.1.0` release (to support semantic version ranges)
    - All feature development will occur on `main` and treated as features to be included in some future `v2.0.0`
        - This includes containerd removal work
        - This includes anything related to notary/discovery/referrers/etc.
- Project board
    - Exactly where (org, repo) TBD
    - Steve introducing Scott to Samir, who did a similar thing for a different project
    - Let's compare notes then just do whatever gives us what we need in the easiest way. Need for now is to be able to connect work needed for the 1.0.0 release, and distinguish from v2 development

## November 18, 2021

### Attendees:
- _add yourself_

### Agenda Items:
- ORAS (Scott Rigby)
- _add your topics_

### Notes:
- _meeting minutes_

## Octoboer 27, 2021

### Attendees:
- Steve Lasker (Microsoft)
- Tejaswini Naduggar(Microsoft)
- Sajay Antony(Microsoft)
- Shiwei Zhang (Microsoft)
- Hector Fernandez (VMware)
- _add yourself_

### Agenda Items:
- [OCI Distribution Extension API](https://github.com/opencontainers/distribution-spec/pull/111) (Teja)
- _add your topics_

### Notes:
- _meeting minutes_


## October 20, 2021

### Attendees:
- Hector Fernandez (VMware)
- Steve Lasker (Microsoft)
- Michael Brown (AWS)
- Sajay Antony
- Shiwei Zhang (Microsoft)

### Agenda Items:
- [hector] Indexing artifacts content to provide better query capabilities across a signle or all artifacts in the repos. 

### Notes:
- _meeting minutes_

## October 13, 2021
### Attendees:
- Sajay Antony
- Shiwei Zhang (Microsoft)
- Michael Brown (AWS)
- Steve Lasker (Microsoft)
- _add yourself_

### Agenda Items:
- [brownxmi@] OCI next steps: suggestion from OCI summit was to submit a proposal for a working group. How should we move forward with gathering feedback from outside this group and incorporating it into our proposal?
- [sajay/Shiwei] - Extension API updates. 
  - [Extensions API for Distribution](https://hackmd.io/8vXj0k1HSIGF2kauCgnroA?view)
  - [Distribution Extension](https://hackmd.io/1zvOVNsvQ3a9D0knPOBrZw?view)
  - [[Display PR] Distribution Extension](https://github.com/shizhMSFT/distribution/pull/1)
  - [[Display PR] ORAS Extension](https://github.com/shizhMSFT/distribution/pull/2)
- [lahiru] - https://github.com/oras-project/artifacts-spec/pull/58
- _add your topics_

### Notes:
- Working group proposal is being updated, with dicussions hopefully happening this week while at KubeCon
- References can already exist without the subject, but we currently reject pushes if the subject doesn't exist
    - lahiru: why do we need to make a constraint to prevent a valid state?
    - steve: we should be prescriptive to provide consistency in expectations, but prescriptive isn't exclusive of options if they're well understood options
    - lahiru: the other case is what happens when the subject digest from the referrers api doesn't exist in the repo
    - lahiru: also, references vs. referrers seems inconsistent
    - sajay: we can change it, should probably create a seperate issue. this might cause friction with some of the clients that have started to implement it.
    - [AI]: create an issue to resolve the consistency issues in the spec & merge the current PR without error
- extensions api discussion during OCI meeting last week
- _meeting minutes_

## October 6, 2021

### Attendees:
- _add yourself_

### Agenda Items:
- [brownxmi@] OCI next steps: suggestion from OCI summit was to submit a proposal for a working group. How should we move forward with gathering feedback from outside this group and incorporating it into our proposal?

### Notes:
- _meeting minutes_


## September 29, 2021

### Attendees:
- Shiwei Zhang (Microsoft)
- Michael Brown (AWS)
- _add yourself_

### Agenda Items:
- Meeting regularity
- https://github.com/oras-project/artifacts-spec/pull/58
- https://github.com/oras-project/artifacts-spec/issues/59
- _add your topics_

### Notes:
- We're at a point of stability with the spec we don't have Will keep the meeting time, but we're at a point of stability 
- _meeting minutes_

## September, 15, 2021

### Attendees:
- Steve Lasker (Microsoft)
- Shiwei Zhang (Microsoft)
- Michael Brown (AWS)
- _add yourself_

### Agenda Items:
- [Artifacts Spec](https://github.com/oras-project/artifacts-spec/) Draft Release Update (Steve)
- Doc Updates to oras.land (Steve)
- Blog Post, on oras.land (Steve)
- 

### Notes:
- _meeting minutes_

## September, 8, 2021

### Attendees:
- Steve Lasker (Microsoft)
- Shiwei Zhang (Microsoft)
- Michael Brown (AWS)
- _add yourself_

### Agenda Items:
- Cutting spec draft.1 - Now that [PR#35](https://github.com/oras-project/artifacts-spec/pull/35) is closed. What's left before we cut draft.1? (Lachlan)
- Open Items for Draft1 or Post draft 1 (group discussion)
- Versioning of Artifacts 1 or 2? (Steve)

### Notes:
- _meeting minutes_

## September 1, 2021

### Attendees:
- Lachlan Evenson (Microsoft)
- Shiwei Zhang (Microsoft)
- Steve Lasker (Microsoft)
- Michael Brown (AWS)
- Sajay Antony (Microsoft)
### Agenda Items:
- Cutting spec draft - What's left? Discussion on process [PR#19](https://github.com/oras-project/artifacts-spec/pull/19) (Lachlan)
- `subject` conversation (Michael)
    - https://hackmd.io/wFmCCyv8Rv6vGY4M_vjjRw?view

### Notes:
- Steve/Lachlan: Clean up release PR & move issues to draft releases. RC releases should be declared once all issues have been fixed.
- `subject` conversation: https://hackmd.io/wFmCCyv8Rv6vGY4M_vjjRw?view
    - pointing to blobs would be a breaking change in the future.
- Take a look at oras-project/distribution PR: https://github.com/oras-project/distribution/pull/8


## August 25, 2021

### Attendees:
- Justin Cormack (Docker)
- Steve Lasker (Microsoft)
- Michael Brown (AWS)
- Lahiru Dissanayake (AWS)
- Shiwei Zhang (Microsoft)
- Sravan Rengarajan (AWS)
- Sajay Antony (Microsoft)

### Agenda Items:

- Release manager process (Sajay)[PR#8](https://github.com/oras-project/community/pull/8)
- Lifecycle Management in artifact spec (Lahiru) [Issue#20](https://github.com/oras-project/artifacts-spec/issues/20)
- _add your topics_

### Notes:
- Lifecycle management
    - Agreement to change SHOULD to MAY to reduce concerns around conformance tests. Also agreed to remove refernces to ref-count. The secion would remain in the same artifact-manifest.md doc to avoid having too many docs, but reudced content.
- _meeting minutes_


## August 18, 2021

### Attendees:
- Tejaswini Duggaraju (Microsoft)
- Steve Lasker (Microsoft)
- Shiwei Zhang (Microsoft)
- Michael Brown (AWS)
- Aviral Takkar (Microsoft)
- Lahiru Dissanayake (AWS)
- Sajay Antony (Microsoft)
- _add yourself_

### Agenda Items:
- What's left to cut a 1.0 RC release of the artifacts-sepc? (Steve)
    - Triage the [list of issues](https://github.com/oras-project/artifacts-spec/issues)
- [PR #9 - Add @michaelb990 as an owner](https://github.com/oras-project/artifacts-spec/pull/9) (Sajay/Michael)
- [PR #17 - Add go spec](https://github.com/oras-project/artifacts-spec/pull/17)(Aviral/Sajay)
- _add your topics_

### Notes:
- [ORAS Projects/Release](https://github.com/oras-project/artifacts-spec/projects/1)
- _meeting minutes_

## August 11, 2021

### Attendees:
- Sajay Antony (Microsoft)
- Justin Cormack (Docker)
- Michael Brown (AWS)
- Tejaswini Duggaraju (Microsoft)
- Shiwei Zhang (Microsoft)
- Steve Lasker (Microsoft)
- Sravan Rengarajan (AWS)
- Aviral Takkar (Microsoft)

### Agenda Items:
- [Discuss the `referrers` api payload PR](https://github.com/oras-project/artifacts-spec/pull/3) (Steve/Michael)
    - [Discussion #7](https://github.com/oras-project/artifacts-spec/discussions/7)
- [Paging API](https://github.com/oras-project/artifacts-spec/issues/4) (Michael)
- Working group next steps (Michael)
- Getting additional maintainers on the sub-project (Sajay) 
- _add your topics_