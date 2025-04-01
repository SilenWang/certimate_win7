[![BUILD](https://github.com/SilenWang/certimate_win7/actions/workflows/build.yaml/badge.svg?event=schedule)](https://github.com/SilenWang/certimate_win7/actions/workflows/build.yaml)

[中文](README.md) | [English](README_EN.md)

> [!WARNING]
> This project only compiles the Win7-compatible version of Certimate and has not performed any unit-tests. It does not guarantee that all original features are available.

# Certimate-Win7

[Certimate](https://github.com/usual2970/certimate) is a very useful automatic certificate deployment tool. However, it depends on Go version 1.23 or higher. Since Go version 1.21 no longer supports older systems such as Win7/Windows Server 2008, the official releases cannot be used on these systems. The servers in my company are running on these outdated systems, and they only support the RDP protocol. It is inconvenient to open other services to receive and deploy certificates.

Therefore, this project aims to use a [third-party Win7-compatible Go version](https://github.com/XTLS/go-win7) to compile Certimate and generate executable programs for Windows.

## Todo

- [x] Write the initial Release Workflow
- [x] Manually specify the latest version v2 and build the release.
- [x] Modify the Workflow to track releases from the original repository and generate corresponding compatible versions