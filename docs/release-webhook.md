# Release webhook

Set the repository Actions secret `RELEASE_WEBHOOK_URL` to your receiving
workflow's HTTPS webhook URL. Whenever a release or prerelease is published,
GitHub Actions sends a JSON POST with `tag` (the release tag) and `release_notes`
(the release body as Markdown, or an empty string if no notes were provided).
It also sends `content`, combining the tag and release notes for receivers that
expect a standard message field. Saving a draft or pushing a tag alone does not
send a webhook.
