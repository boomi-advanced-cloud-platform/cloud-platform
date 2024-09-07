
# Change Log
All notable changes to this project will be documented in this file.
 
The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).
 
## [1.2.177] - 2024-06-04

### Added
- Added support for BGP routing for S2S VPNs. (#80)

## [1.2.163] - 2024-05-02

### Changed
- Updated Local Disk to XFS to overcome inode limitations of EXT4 (#74)

## [1.2.157] - 2024-04-29

### Added
- Added and published available knowledgebase including FAQ, architecture design and key configuration information (#60)

### Changed
- Removed VPN connection configuration from deployment and moved to Runbook to allow for multiple customised connections. (#51)

## [1.2.139] - 2024-04-25

### Changed
- Updated Molecule configuration to use volume claim templates. (#71)

## [1.2.137] - 2024-04-25

### Added
- Added presistent storage with Azure Premium Disk for Boomi to increase the speed of certain file read/write operations (#69)

## [1.2.128] - 2024-04-24

### Changed
- Updated the AKS cluster and node version from 1.27.3 to 1.28.5

## [1.2.120] - 2024-04-23

### Added
- Added Prometheus to client subscriptions to allow for real-time CPU/Memory usage monitoring (#13)
 
## [1.2.117] - 2024-04-20
 
### Added
- Added the changelog
- Added a Shared Pod - Github Self-Hosted Runner (#52)
- Added a Shared Pod - LetsEncrypt Certrotation (#1)
- Added a Shared Pod - Octopus Deploy Tentacle (#2)
- Added new function to create IP allow-lists per domain (#17)
 
### Changed
- Enabled Firewall logging (#15)
- Enabled Azure Front Door logging (#16)
 
### Fixed
- Fixed an issue preventing Ingress Configuration with Azure Front Door to be automated (#28)
- Fixed an issue in CICD Deployment where Memory and CPU limits were too low (#57)
- Fixed an issue with VPN Client Configuration to avoid communication issues to client network (#50)
- Fixed an issue which prevented custom domains (vanity urls) to access the Web Application Firewall (#18)
- Fixed an issue causing Atom/Molecule Pods to hang (#20)
- Fixed an issue preventing Octopus Deploy Tentacle from updating (#45)
- Fixed an issue preventing pods from pulling images from the Azure Container Registry (#49)

### Security
- Action Code Verification Test results (#23, #24)
- Updated Kubernetes Admin to disallow access from untrusted sources (#14)
- Implemented manual approval steps for deploying to shared services (#21)
