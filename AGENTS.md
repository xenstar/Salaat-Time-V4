# AGENTS.md - Salaah Time V4 Releases

This repository is the public, binary-only release channel for Salaah Time V4.
Source code and development instructions belong in the private source
repository.

## Repository scope

- Keep this repository focused on public release documentation, release assets,
  and updater metadata.
- Publish only verified NSIS installers, their blockmaps, `latest.yml` updater
  metadata, and user-facing release notes.
- Treat every file committed or uploaded here as public.

## Prohibited content

- Never publish source code, unpacked application builds, dependencies,
  environment files, credentials, tokens, secrets, or internal infrastructure
  details.
- Never publish personal, customer, collaborator, or business information.
- Never publish internal planning notes, behavioral profiles, local filesystem
  paths, or private repository content.
- Never upload debug builds, test-only artifacts, or an unverified installer as
  the latest public release.

## Release checks

Before publishing a release:

1. Confirm the installer version matches the approved release version.
2. Run the required checks and installed-build validation for that exact build.
3. Calculate and record the installer SHA-256.
4. Verify that the installer, blockmap, and `latest.yml` refer to the same file,
   version, size, and hash.
5. Use hyphenated artifact names. Do not rename assets after updater metadata is
   generated.
6. Mark a release as Latest only after the installer and updater metadata have
   both been verified.
7. Keep release notes factual, user-facing, and limited to fixes or features
   present in the published build.

## Allowed release assets

- `Salaah-Time-V4-<version>.exe`
- `Salaah-Time-V4-<version>.exe.blockmap`
- `latest.yml`

Do not attach ZIP archives, portable folders, source archives, or unpacked
application directories unless the release policy is explicitly changed.

## Change discipline

- Inspect the repository status before editing or publishing.
- Commit and push documentation through the currently approved Git workflow.
- Do not force-push or rewrite release history without explicit approval.
- Recheck the public diff before pushing for personal or sensitive information.
