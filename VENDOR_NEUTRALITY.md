# ORAS Vendor Neutrality Declaration

As a Cloud Native Computing Foundation project, ORAS maintains strict [vendor neutrality](https://contribute.cncf.io/maintainers/community/vendor-neutrality/).

## Registry Vendor Neutrality

ORAS is designed to work with any OCI-compliant container registry regardless of vendor. The project supports all registries that implement the [OCI Distribution Specification](https://github.com/opencontainers/distribution-spec), including:

- Cloud-hosted registries (Azure Container Registry, Amazon ECR, Google Artifact Registry, Docker Hub, Quay, GitHub Container Registry, etc.)
- Self-hosted registries (Harbor, Zot, distribution/distribution, etc.)
- Enterprise registries (JFrog Artifactory, Sonatype Nexus, etc.)

ORAS focuses on open, vendor-neutral specifications (OCI Distribution Spec, OCI Image Spec, OCI Artifacts) to ensure artifacts can be stored, distributed, and retrieved across any compliant registry. While ORAS may provide guidance for registry-specific configuration or authentication patterns, all core functionality operates through standardized OCI APIs without requiring vendor-specific features.

## Feature Vendor Neutrality

All ORAS features are developed to work uniformly across OCI-compliant registries:

- **Authentication**: Supports standard OCI registry authentication mechanisms (OAuth2, basic auth, bearer tokens) without requiring vendor-specific credential providers
- **Artifact Types**: Works with any artifact type following OCI specifications, not limited to specific vendors or use cases
- **Reference Types**: Implements OCI reference types (formerly artifacts-spec) in a vendor-neutral manner
- **CLI and SDKs**: Designed to provide consistent behavior across all registries that comply with OCI specifications

No ORAS feature requires a commercial registry service or vendor-specific API to function. Users can deploy and operate ORAS entirely with self-hosted, open-source registries.

## Specification Vendor Neutrality

ORAS actively contributes to vendor-neutral specifications:

- Participates in the [OCI (Open Container Initiative)](https://opencontainers.org/) to develop and maintain open standards
- Collaborates across vendors, cloud providers, and open-source communities to ensure specifications serve broad use cases
- Maintains the [OCI Artifacts specification](https://github.com/oras-project/artifacts-spec) as a vendor-neutral approach to storing arbitrary artifacts in OCI registries

## Development Vendor Neutrality

The ORAS community prioritizes vendor-neutral development infrastructure:

- **CI/CD**: Utilizes GitHub Actions and CNCF-provided infrastructure for continuous integration and testing
- **Testing**: Validates functionality against multiple registry implementations (both commercial and open-source) to ensure vendor neutrality
- **Community Resources**: Hosts community meetings, documentation, and communication channels using vendor-neutral platforms (CNCF Slack, public GitHub repositories, oras.land)

While some development and testing resources are contributed by maintainer organizations, the project maintains independence by:
- Not requiring any single vendor's registry or infrastructure for core development
- Testing against a diverse set of registry implementations
- Ensuring all released artifacts and distributions are available through public, vendor-neutral channels

## Governance Vendor Neutrality

ORAS governance ensures no single vendor can control the project direction:

- As specified in [GOVERNANCE.md](./governance/GOVERNANCE.md), no single company or organization can employ a simple majority of the org owners
- Decision-making follows lazy consensus and voting processes that prevent vendor lock-in
- All subprojects maintain independent maintainer teams with diverse organizational representation

This commitment to vendor neutrality ensures ORAS remains an open, collaborative project serving the entire cloud-native ecosystem.
