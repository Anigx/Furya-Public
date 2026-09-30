# Furya Account and Data Deletion

Last updated: September 30, 2026

**App:** Furya, including the Google Play app `com.anigx.furya` and existing
sideload editions. **Operator:** Anigx.

## Request deletion without installing the app

Email **[Anigx@pushedv.de](mailto:Anigx@pushedv.de?subject=Furya%20account%20or%20data%20deletion)**
with the subject **Furya account or data deletion**. This is a private request
channel; do not post account information in a public GitHub issue.

1. Say whether you want to delete your **Furya community account**, specific
   community content, or identifiable **usage statistics/crash reports only**.
2. For a community account, provide its board pseudonym and, if available,
   the linked source/username or Telegram username so we can locate it.
   A username alone is not sufficient proof of ownership.
3. For statistics, provide the installation ID if you still have it. For crash
   reports, provide app version, approximate event time and device context to
   help locate an identifiable event. You do not need to create a community
   account to ask about optional telemetry.
4. We will verify ownership privately before erasing account data. This can
   require confirmation through the existing identity or a one-time proof on
   a linked source profile. **Never send passwords, API keys, session/refresh
   tokens or recovery codes.** If you cannot access an identity, explain this
   so we can assess another reasonable verification method.

We normally address requests within 30 days, subject to necessary identity
verification and applicable legal requirements. If pseudonymous telemetry
cannot be linked to the supplied information, we will explain that limitation;
its automatic retention/expiry still applies.

## Delete from an updated app

Builds containing the privacy updates after version 1.6.0 provide:

**Settings → Storage & Data → Privacy Controls → Privacy & Account Deletion →
Delete community account**.

Sign in with Telegram if needed and confirm deletion. You do not need to
re-link a source just to erase the Furya Auth account. If your build does not
yet have this screen, use the email request above; the backend deletion
service is already deployed.

## What is erased and what can remain

- Erased: Furya Auth account/identities/sessions/refresh state, community
  profile, linked-source identities, roles, individual votes, associated
  content-report/rate-limit records, account-owned file attachments and
  relevant linked legacy private reports.
- Your authored request/comment text is replaced by a deleted placeholder.
  Other authors' discussion and deleted placeholders can remain.
- Relevant moderation actions retain the action/context without the erased
  actor or arbitrary metadata and expire under the retention policy.
- Isolated backups and retired Furya copies have a 30-day expiry and are
  removed by scheduled maintenance. They are not used as an active service;
  erasure must be re-applied if an older copy is restored before expiry.
- Optional statistics use a separate installation ID; ask for those separately
  when identifiable. Statistics/version history expire after 90 days and
  private Furya crash-diagnostic copies after 30 days. Sentry-hosted copies use
  the project's retention/provider terms; contact us about identifiable events.

This does not delete an independently managed Telegram/e926/e621/e6ai account,
local app data/downloads, exports you made, or copies already made by others.
For personal references in another author's text, identify the content in a
private request so it can be reviewed.

See the [Furya Privacy Notice](PRIVACY.md) for the complete data/retention scope.
