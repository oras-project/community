# Working Groups

Working Groups are organizations responsible for the design and implementation of large architectural aspects of the overall ORAS project. Working Groups operate with a fair amount of autonomy within the broader scope of the project. They tend to be long-lived or temporary.

Working Groups are primarily used to facilitate topics of discussion that are in scope for ORAS but that cross multiple sub-projects and teams. It provides a formal avenue for disparate teams or groups to collaborate around a common problem, craft a balanced position, and disband. 

Generally, Working Groups could be created once sufficient community interest and discussion has occurred that there is general agreement that:

- The problem or feature space is interesting and is worth long-term investment by the ORAS community
- The problem or feature space is not well-covered by any of the existing subprojects or Working Groups
- The problem or feature space is in the scope of ORAS charter but there is not standard solution in the industry yet. It is an innovation work that requires early research and investigation across different organizations

## Purpose of establishing ORAS Working Group

Establishing an ORAS Working Groups enables the ORAS community to experiment, validate, and define new capabilities of specifications. Each Working Group shall have a defined scope of the ORAS Working Group's intended activities and goals. The end result of the Working Group's work product shall be either:

- an update to an existing specification (for example, adding support for a new set of features);
- a new specification (for example, creating an specification for a new topical area); or
- a new ORAS sub-project other than a specification (for example, creating a reference implementation of an specification).

Any participant in the ORAS community may propose a Working Group to the maintainers. Participants can become maintainers of the Working Group. The maintainers shall maintain a public list of the information required to be included in a Working Group proposal.

## Required information for ORAS Working Group Proposal

An ORAS Working Group proposal should contain the following information:

- a charter with mission, goals, and scope of what the Working Groups aims to accomplish
- a list of owners who have agreed to participate in the Working Group, review progress, report - progress back to the ORAS community, and present the results to the maintainers once the Working Group has completed its objectives
- a list of ORAS projects, non-ORAS projects, or organizations sponsoring the Working Group and participating in the implementation and use case validation of the work done by the group
- a set of project rules which govern how contributions to the Working Group will be handled and decisions will be made
- a working agreement for making progress, which may include weekly meetings, dedicated channels for discussions, or a shared repository
- a request for ORAS resources, which may include recurring meetings in the ORAS calendar, ORAS hosted repository, or topic specific communication channels
- a name of the Working Group

> Note: It is recommended that the Working Group is clearly differentiated from the sub-projects by using "Working Group" in the name and `wg-` prefix for the designated repository if such is required.
Proposal for a Working Group should be submitted as a GitHub issue with all the information above.

## Requirements for maintainers approval of the Working Group

ORAS maintainers should review the proposal for a Working Group and vote for its creation. Working Groups can be approved with a super-majority of the maintainer votes. Once the approval is complete, maintainers will provide the requested resources to the Working Group participants.

## Required information for maintainers approval of the Working Group outcome

When a Working Group determines that it has completed its initial work and is prepared to request maintainers approval for the outputs as a specification or a sub-project for ORAS, the Working Group owners will present to following content to the ORAS maintainers:

- the recommended next steps, draft specification, or project content
- the validation work which demonstrates real world usability
- the set of maintainers who have agreed to carry the work forward

There is no requirement that owners or contributors to the ORAS Working Group will continue to be maintainers for an approved specification or other ORAS sub-project after maintainers approval and release. However, the maintainers will consider it a requirement that any approved specification or other ORAS sub-project has a dedicated and active group of maintainers to continue the work.

## Dissolving a working group

Some Working Groups are ephemeral or naturally reach the end of their useful life. Working Group owners can choose dissolve their Working Groups by submitting an issue in the ORAS community repository. The ORAS [Owners](../OWNERS.md) takes ownership to handle their request and ORAS Owners also reserves the right to dissolve or recharter working groups over time as necessary, though they will strive to first discuss this in committee meetings and open community discussion.

## Attributions

The Working Group model we created above references the practice from [OCI Working Groups](https://github.com/opencontainers/tob/blob/main/WG-INFO.md), [Knative working group processes and guidelines](https://github.com/knative/community/blob/main/mechanics/WORKING-GROUP-PROCESSES.md) and [Kubernetes Working Group Formation and Disbandment](https://github.com/kubernetes/community/blob/master/committee-steering/governance/wg-governance.md).
,m 