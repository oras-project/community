# ORAS Roadmap

The ORAS community has triaged the GitHub issues and confirmed the timeline and roadmap for ORAS as follows. You can also find the detailed GitHub issues and status in each milestone from the [ORAS planning board](https://github.com/orgs/oras-project/projects/2/views/2). We are open for new proposals and feature requests from the community.

## Timeline

| Release | ETA Date |
| --- | --- |
| ORAS 0.15.0 | Sep 2022 |
| ORAS 0.15.1 | Oct 2022|
| ORAS 0.16.0 | Oct 2022 |
| ORAS v1.0.0-rc.1 | Nov 2022 |
| ORAS v1.0.0 | Jan 2023 |

| Release | ETA Date |
| --- | --- |
| ORAS-go v2.0.0-rc.4 | Oct 2022 | 
| ORAS-go v2.0.0-rc.5 | Nov 2022 |
| ORAS-go v2.0.0 | Dec 2022 |

## Milestone

|Area | Feature or user story | Milestone |  Status | Related issue/design |
| --- | --- | --- | --- |  --- |
|Repository |- List repositories of a registry </br> -  List tags of a repository|0.15 | WIP| [CLI UX design](https://hackmd.io/aLxws7mhSZukfFzx3PKq3w?view#Repository--Tags) |
|Tag |- Tag a manifest with single tag </br> - Tag a manifest with multiple tags </br> - Push multiple tags in one time |0.15 |WIP| [CLI UX design](https://hackmd.io/aLxws7mhSZukfFzx3PKq3w?view#Repository--Tags) |
|Manifest | Upload, fetch, delete a Manifest |0.15 |WIP| [CLI UX design](https://hackmd.io/aLxws7mhSZukfFzx3PKq3w?view#Blob) |
|Blob| Upload, fetch, delete a Blob |0.15 |WIP| [CLI UX design](https://hackmd.io/aLxws7mhSZukfFzx3PKq3w?view#Blob) |
|E2E Testing | Build end-to-end tests to continuously validate the usability of ORAS CLI features | 0.16 |  WIP | [ORAS #523](https://github.com/oras-project/oras/issues/523)
|OCI Support | Support the OCI reference types | 0.16 | To do | [ORAS-go #271](https://github.com/oras-project/oras-go/issues/271) |
|Custom http header | Support customer-defined http headers | 0.16 | To do | [ORAS #503](https://github.com/oras-project/oras/issues/503)
| Push / Pull Artifacts | Push / Pull Artifacts from OCI Image Layout | v1.0.0 | To do | [ORAS #378](https://github.com/oras-project/oras/issues/378)
| ORAS login | ORAS CLI remove dependency on Docker CLI | v1.0.0 |To do | [ORAS #414](https://github.com/oras-project/oras/issues/414) |
| Export manifest descriptor | Export manifest descriptor by ORAS push | v1.1.0 | Initial implementation | [ORAS #497](https://github.com/oras-project/oras/issues/497)
| SDK | Provide ORAS .NET SDK | Future | Discussion | 
| Pull Artifacts | support ``--output -`` to pull to stdout | Future |  Discussion | [ORAS #346](https://github.com/oras-project/oras/issues/346) | 
| Search artifacts | Provide search capabilities for the stored artifacts | Future |  Discussion | [artifact-spec #72](https://github.com/oras-project/artifacts-spec/issues/72)
| UX | Revisit and Simplify the Design of ORAS | Future |  Discussion | [oras #304](https://github.com/oras-project/oras/issues/304) |
| SDK (Multi-tenancy) | Repository level auth provider support | Future | Discussion | Depends on multi-tenant user scenario | [oras-go #136](https://github.com/oras-project/oras-go/issues/136)
| SDK (Performance) | Stop sending network requests for fetching chunked blobs | Future |  Discussion | [oras-go 126](https://github.com/oras-project/oras-go/issues/126)|

