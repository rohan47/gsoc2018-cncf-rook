# Google Summer of Code 2018 - Add Network File System (NFS) as a Rook storage backend(CNCF)

Final submisision Summary.

## Project Abstract
Rook is an open source orchestrator for distributed storage systems running in kubernetes, currently in alpha state and has focused initially on orchestrating Ceph on top of Kubernetes. There is no option for Network File System (NFS) yet.
This project aims to add NFS as another storage backend.

## Project Mentors

[Jared Watts](https://github.com/jbw976/)  
[Travis Nielsen](https://github.com/travisn)

## General Info
Name: Rohan Gupta  
Email: rohanrgupta1996@gmail.com  
Blog: [rohan47.tech](rohan47.tech)  
Slack nick: rohan47 (rook-io.slack.com)  
Github: [rohan47](https://github.com/rohan47)  
Twitter: [@rohanrajgupta](https://twitter.com/rohanrajgupta)  

## Links
[Project Proposal](proposal/)  
[Project on GSoC site](https://summerofcode.withgoogle.com/projects/#5926207925780480)  
[Feature request for this project](https://github.com/rook/rook/issues/1551)  

## Tasks
### Phase 1/ First evaluation
- [x] Investigate related technology such as Kubernetes, NFS servers, volume provisioning, etc.
- [x] Identify full scope and requirements of feature
- [x] Prototype as needed to explore potential implementation choices and trade-offs
- [x] Write detailed design document that specifies how feature will be implemented and tested
- [x] Submit a pull request for the design, integrate feedback and have it approved and merged to master
- [x] New types, custom resources, and config options to capture the full experience for a user to setup and configure NFS storage with Rook

### Phase 2/ Second Evaluation
- [x] NFS server deployment that will use the provided backing storage (host path, persistent volumes, CephFS) and handle NFS client requests for storage operations via the NFS protocol via NFS operator in response to CRD add event
- [x] Service creation for external access of storage
- [x] Documentation for app/pod consumption of NFS storage (static provisioning)

### Phase 3/ Third Evaluation
- [x] Author an end to end Integration tests for any completed code/features

## Design Documentation
[Design Proposal: Add NFS to Rook](https://github.com/rook/rook/blob/master/design/nfs.md)  
[Pull Request for the Design](https://github.com/rook/rook/pull/1740)

## User Documentation and Code
[Pull Request: Add NFS to Rook](https://github.com/rook/rook/pull/1783/)
