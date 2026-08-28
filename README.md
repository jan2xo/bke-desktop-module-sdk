# BKE Desktop Module SDK

STATUS: SCAFFOLD / PRE-API

This repository will eventually contain the reusable mechanics for BKE desktop module integration, including supported module launch, enterprise child-session redemption, and secure IPC framing. The current package is foundation scaffolding only.

## What this package is not

This package does not currently define a public module API, launch policy, executable selection, entitlement authority, licensing authority, privileged execution, trusted keys, or product policy. The Licensing Agent remains the local authority for supported operations.

The public API is intentionally not frozen. Future implementation will be extracted from certified, working BKE products and Agent protocols only after evidence review. No Air Stack, Render Dock, or Licensing Agent implementation is copied here.

## Package

Package ID: BKE.Desktop.ModuleClient  
Version: 0.1.0  
Target: net8.0-windows

The package is an unpublished CI artifact candidate. Configure a package source only after an approved distribution mechanism exists.

## Development

The repository uses the .NET 8 SDK policy in global.json. The solution contains a packable library project and a real test project. Functionality will be added in a later, evidence-driven phase.

## Security boundary

Consumers will not use this package to select arbitrary executable paths or trusted policy. The SDK will remain integration infrastructure; authority stays with the Licensing Agent and BKE environment.
