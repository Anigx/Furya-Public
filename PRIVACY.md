# Furya Privacy Notice

Last updated: July 28, 2026

## Scope

This notice describes information handled by the Furya Android app, its public Community Feedback Board, and Furya's existing private in-app report dialog. It does not replace the privacy practices of e621, e6ai, GitHub, Supabase, or any other service you use through Furya.

## Information stored on your device

Furya stores app data locally, which can include account preferences, source selection, filters and blacklist entries, local favorites, collections, search history, cached posts and tags, and downloaded media. e621 and e6ai usernames and API keys used by the app are stored on the device in secure storage for source-account access.

Community-account session and magic-link sign-in state are also stored on the device so the app can maintain the community session.

## e621 and e6ai account use

Furya sends requests directly to the e621.net and e6ai.net APIs when you use those sources. Depending on what you do, those requests can include authentication, searches, tag lookups, favorites, pools, downloads, and blacklist operations.

To participate in the Community Feedback Board, you must link at least one e621 or e6ai account. During linking, Furya verifies the account over TLS and records the verified external account identity needed for the link. Furya does not store the source API key or password used to perform that verification. Those credentials are not displayed on the board.

## Community Feedback Board

The board is publicly readable. If you participate, the following information can be public:

- Your board pseudonym.
- Request titles and descriptions.
- Comments you submit.
- Aggregate vote scores and discussion context.
- Attachments only after a moderator approves them for public display.

Furya also handles the confirmed email address used for magic-link community sign-in, the community account identifier, the linked e621/e6ai identity, your acceptance of the Community Rules and this notice, votes, content reports, and moderation-related records needed to run the board. Your email address and linked source-account names are not used as your public board pseudonym.

Before approval, board attachments are held privately for moderation. Only approved attachments are made available on the public board. Do not upload credentials, personal data, source media, or other information that should remain private. See [Community Rules](COMMUNITY_RULES.md).

## Private in-app reports

Furya's existing in-app report dialog is separate from the public board. It sends private bug or feature reports to Furya's report system. A report can include its type, title, description, optional reproduction steps, app version and build number, platform, locale, optional Android device model, and the screen context. It can also include the available e621/e6ai user context or guest status. If optional analytics is enabled and an installation ID is available, that ID can be included.

Private reports are not published on the board and are not migrated into it. Do not include API keys, passwords, or other secrets in a report.

## Optional analytics

Optional analytics is consent-based and can be configured in Settings. When enabled, Furya may send the selected device information, installation ID, app version, and language to Supabase for app-usage and version analytics. Analytics is optional; declining or withdrawing the applicable options prevents the corresponding analytics fields from being sent.

## Other services

Furya communicates with:

- **e621.net and e6ai.net** for the content-source features you choose to use.
- **GitHub** to check Furya releases and updates; the app sends its current app version for that check.
- **Supabase** for optional analytics, private in-app reports, and the community account and feedback-board services.

These services handle information under their own terms and privacy practices.

## Anonymization and deletion

Removing a board item or deleting a community account anonymizes its author. The request, discussion, and vote history may remain for context; attachments are removed. This does not make content that was already public private again.

To remove local app data, remove connected source accounts in Furya, clear app storage or cache as appropriate, delete downloaded media, and uninstall the app. Local-data removal does not delete data already sent to e621, e6ai, GitHub, Supabase, or the public board.

## Security and contact

Protect your device and never share API keys, passwords, magic links, or authentication tokens. Do not put sensitive information in public GitHub issues.

For privacy questions or account/content anonymization requests, open an issue in the [Furya Public GitHub repository](https://github.com/Anigx/Furya-Public/issues). GitHub issues are public, so provide only the information needed to describe the request. For security vulnerabilities, follow [SECURITY.md](SECURITY.md).