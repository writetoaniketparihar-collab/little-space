# Downloads and installer verification

## Official downloads

Buy through [littlespace.pro](https://littlespace.pro/). Existing customers can download through the [Polar customer portal](https://polar.sh/little-space/portal), using their purchase email.

This repository does not host paid installers, license keys or customer download links. Do not download replacement installers from issue comments or third-party attachments. Support will not ask you to reveal passwords, disable Gatekeeper or remove system security protections to install Little Space.

## Verification record

On 7 November 2026, the Little Space 1.4.1 disk image passed:

- Digital signature verification with `codesign --verify --strict`.
- Stapled notarization-ticket validation with `xcrun stapler validate`.
- Gatekeeper assessment with `spctl --assess`, reporting `Notarized Developer ID`.

Reference file: `Little-Space-1.4.1.dmg`

SHA-256:

```text
9bb12e0ceacb487861b1230a58fdea10360a0da131cf3ebcafc3154f582903a1
```

This checksum applies only to that exact disk image, not to other versions or repackaged files. This record does not assert that the customer portal has already been updated to this version. The version offered by the portal may differ.

To compare a downloaded copy of that version on your Mac:

```sh
shasum -a 256 "$HOME/Downloads/Little-Space-1.4.1.dmg"
```

Check the filename and location first. A matching checksum establishes a match to the reference file; it does not establish that software has no bugs or vulnerabilities. If the checksum differs, do not override a macOS warning. Contact [hello@littlespace.pro](mailto:hello@littlespace.pro) with the version and warning text.
