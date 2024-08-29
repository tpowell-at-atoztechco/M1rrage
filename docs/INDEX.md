# M1rrage Documentation
This documentation explains how M1rrage works, in addition to release notes regarding upcoming releases and platform-specific setup guides. This documentation is and should continue to be beginner-friendly.
## Introduction
M1rrage is a series of tools and configurations designed for using QEMU to emulate macOS on simulated Apple Silicon. It is only for educational use and is not intended for professional use or to defraud Apple of the money they make primarily through hardware sales.
## Supported Platforms
M1rrage is supported on the following platforms:
- QEMU [ Howto: Download | Compile | Setup ]
- Proxmox [ Howto: Download | Compile | Setup ]
- Docker [ Howto: Download | Compile | Setup ]
- <i>Add your QEMU-centric platform here!</i>
## Release Channels
- Source
  The raw, uncompiled source code. Users are expected to build the software themselves. This is often the most direct way to access the latest features but requires technical expertise.
- Snapshot
  A snapshot of the codebase at a specific point in time, used for ongoing development. These are less stable but provide a current view of the project.
- Unstable
  A channel that includes recent changes that have not been thoroughly tested. These releases are not recommended for production use but are available for those who want to experiment with the latest features.
- Rolling Release
  A continuously updated channel where software is regularly updated without a fixed release schedule. This approach ensures users always have access to the latest version, but it might be less stable.
- Bleeding Edge
  A channel similar to "unstable" or "nightly," where users can access the most recent changes, including experimental features. This channel is for advanced users who are willing to encounter bugs.
- Community
A release that is maintained and tested by the community rather than by a formal development team. The stability can vary, but it relies heavily on community contributions and testing.
- Experimental
  A channel where new, potentially disruptive features are tested. These builds are not stable and are intended for users who want to contribute to testing new ideas.
- Master/Trunk
  Often the main branch of the version control system, where the latest development changes are committed. It may not always be stable, but it is the primary working version of the code.
- User-Contributed
  Releases created by users or community members, often including patches, modifications, or custom builds. These are not officially supported by the core development team.
- Deprecated
  Older versions that are no longer maintained or supported. These are kept for historical purposes or for users who need a specific version but are not recommended for current use.
## Development, issues, pull requests
Please feel free to make contributions and publish commits, and we'll review it and pulish it in accordance with our release policy.
