# Firmware

This repository publicly hosts the firmware of Zenit Astronomy products. Every
version is published as a [release](https://github.com/Zenit-Astronomy/Firmware/releases)
with its update file attached.

## Products

| Product | Release tags | Current release | Changelog |
|---|---|---|---|
| Zenit Align Mini | `zam-<version>` | [0.1.0-rc3](https://github.com/Zenit-Astronomy/Firmware/releases/tag/zam-0.1.0-rc3) (2026-11-13, release candidate) | [zam/changelog.md](zam/changelog.md) |

## Updating a device

1. Download the `.raucb` update file attached to the product's release.
2. Open the device's web interface and install the file from its update page.
3. The device restarts into the new version once the update is installed.

## Release webhook

Set the repository Actions secret `RELEASE_WEBHOOK_URL` to your receiving
workflow's HTTPS webhook URL. Whenever a release or prerelease is published,
GitHub Actions sends a JSON POST with `tag` (the release tag) and `release_notes`
(the release body as Markdown, or an empty string if no notes were provided).
Saving a draft or pushing a tag alone does not send a webhook.
