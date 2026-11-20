# Release webhook

Set the repository Actions secret `RELEASE_WEBHOOK_URL` to your Discord
channel's HTTPS webhook URL. Whenever a release or prerelease is published,
GitHub Actions posts the tag and Markdown release notes with link previews
disabled. Notes that would exceed Discord's message limit are attached as a
Markdown file. If the notes end with this repository's GitHub comparison URL
(including GitHub's generated **Full Changelog** footer), the action posts it
separately after the notes so Discord can preview it. Saving a draft or pushing
a tag alone does not send a webhook.
