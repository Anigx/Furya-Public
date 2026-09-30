# Furya Privacy Notice

Last updated: September 30, 2026

## 1. Operator and scope

Furya is an independent Android client operated under the project name
**Anigx**. For privacy, support, access or deletion requests, contact
**[Anigx@pushedv.de](mailto:Anigx@pushedv.de)**. Use this private contact rather
than a public GitHub issue for account information.

This notice covers the Furya app and Furya-operated services. The announced
scope of the Google Play app, **Furya (`com.anigx.furya`)**, is e926 with the
optional community, statistics and crash-reporting features. Existing
sideload releases also support e621 and e6ai. Available sources and controls
depend on your app build. Furya is not operated by those content sources,
Telegram, GitHub or Google Play.

The backend account-deletion service and the external request process
described below are available now. The new in-app privacy/deletion screen and
statistics corrections are source updates after version 1.6.0 and require a
build that includes them. If your installed version lacks a control, use the
private contact or [external deletion instructions](ACCOUNT_DELETION.md).

## 2. Information stored on your device

Furya stores settings, filters, blacklist entries, saved searches and local
search history, favorites, collections, favorite artists/tags, feed read
state, cache/offline metadata and downloaded media on your device. Its local
statistics screen does not by itself upload those local statistics.

Source usernames/API keys, community-session tokens and temporary PKCE
sign-in state use secure credential storage. Other preferences and content
caches do not all use that secure store. Online actions can transmit related
information even when the app also keeps a local copy.

You can clear local data using app controls or Android's clear-storage
function. Exported/downloaded files outside app storage and copies shared
with others must be removed separately. Clearing storage or uninstalling
does not delete remote accounts or server records.

## 3. Content sources and connected accounts

Furya sends requests to the selected content source and its media hosts.
Depending on the feature, these include search tags/filters, post/pool/artist
identifiers, media requests, source-account identifiers and credentials,
favorites, votes, comments you submit, and blacklist operations. Selected
background feed and offline synchronization features also contact the source.
Source requests use a Furya project/version User-Agent.

Source operators receive your IP address and request metadata and operate
their accounts, content and logs under their own privacy practices. Comments
you submit to a source can be public under your source username. Connecting
or disconnecting a source in Furya does not create or delete that source
account.

For community account linking or recovery of an existing linked profile,
Furya additionally sends the selected source username and API key to its own
HTTPS backend. The backend verifies the account with the source and stores
the source, verified account ID and normalized username. The verification
implementation does not store the API key or a source password in its
database. Do not include those credentials in posts or support requests.

## 4. Telegram and the Community Feedback Board

The board can be read without a community account. Posting, commenting and
voting require Telegram OAuth/OIDC sign-in, a community pseudonym, acceptance
of the Community Rules/notice, and a verified source-account link. Furya does
not ask for your Telegram password.

The authentication service handles the provider identity and returned profile
claims, including name, preferred username, profile-picture URL, verification
flags and sign-in/token metadata. The configured `email_optional` scope can
also return an email address. Furya stores its Auth account/session identity,
community pseudonym, linked-source identity and rules/notice acceptance
version/time. The current flow uses Telegram rather than email magic links;
legacy accounts may retain an older email identity until deleted.

**Public data:** your board pseudonym, published titles/descriptions, comments
and aggregate voting information are readable by others. Furya also keeps
individual votes, access-control, rate-limit, content-report and moderation
records to run and protect the service. Personal details in text remain part
of that text; a pseudonym alone does not make a post anonymous. Do not post
credentials or information you want kept private.

The current client has no image-attachment upload control. The backend's
attachment schema does not mean the app uploads your photo library. Existing
account-owned files, if present on the backend, are included in account erasure.

## 5. Optional usage statistics

Statistics transmission requires consent. You can decline at first start and
change your choices in **Data Sharing Settings**. With statistics enabled,
Furya sends a pseudonymous installation/session identifier, device type and
startup/activity timestamps to its self-hosted service at
`https://api.anigx.de`. Optional fields are device manufacturer/model/Android
SDK version, locale, current app version and version-change history.

New builds use a random installation UUID, not an Android ID. With persistent
ID sharing off, they use a temporary random identifier instead and remove the
previous persistent ID locally. An identifier is still needed for each
statistics request. These identifiers are **pseudonymous, not fully anonymous**.
Turning off the app-version field suppresses both startup version and version
history in builds containing the September 30 correction.

**Older releases through 1.6.0:** the persistent identifier may be derived from
the Android ID; the version-history request was independent of the version
field switch. Declining overall statistics consent stops startup statistics
in those releases too. The corrected builds do not reuse that older ID.

Withdrawing consent stops subsequent startup pings and removes the locally
stored identifier. Corrected builds cancel pending statistics requests and
generate a new ID on later re-consent. Withdrawal does not automatically
delete information already received by the server. See the retention table
and private deletion-request process below.

## 6. Optional crash reports

Crash reporting has its own consent switch and is disabled by default.
Enabling it takes effect after restarting a configured release build.
Disabling it closes the running Sentry SDK. Corrected builds do not initialize
that SDK at startup while crash-reporting consent is off.

When enabled/configured, Sentry receives exceptions, stack traces, release
information, and technical device/operating-system context, including any
SDK-generated technical identifiers. Furya does not set a Sentry user and
disables default PII sending, breadcrumbs, HTTP-request capture, performance
tracing and automatic session tracking. Error messages may nevertheless
contain information related to a failure; those settings do not guarantee
that every possible exception message is anonymous.

Flutter events also produce a limited private copy on Furya's backend:
event ID, release/environment, severity, exception type/message and bounded
stack information. Native crashes are not reliably copied to that database.
Disabling reports does not erase events already submitted. Furya's private
copies expire after 30 days; Sentry-hosted copies are governed by the project's
retention settings and provider processing terms and are used for diagnosing
the relevant failure. Contact us to request removal of identifiable event data.

## 7. Infrastructure and network metadata

- **Self-hosted Supabase software:** Furya authentication, community records,
  optional statistics and private diagnostics. Using this software does not
  mean those records are stored in Supabase's hosted cloud.
- **Cloudflare:** HTTPS edge/tunnel, request delivery and abuse protection for
  the Furya API. Connection metadata includes IP address and coarse country
  derived from IP. This does not use an Android GPS/location permission.
- **Sentry:** opted-in error diagnostics when configured for the build.
- **Telegram:** the sign-in service you choose for community authentication.
- **Content-source operators/media hosts:** source features you use.
- **GitHub:** public project documents, release metadata and sideload assets.

Requests to fixed Furya/source APIs use HTTPS. The corrected Android manifest
disallows cleartext traffic and Sentry configuration requires an HTTPS DSN.
TLS protects device-to-service transmission; this is not a claim that server
operators cannot read data required to provide their service.

Network services necessarily process IP addresses and request metadata for
delivery/security. Furya does not retain Docker stdout/request logs after
the September 30 backend update; Auth security audit records remain subject
to the retention table. Provider-operated services may process connection
metadata under their own service/processing and privacy terms and may process
data outside your country. Furya's service providers process operational data
for the requested delivery/diagnostics purpose; independent source, Telegram
and browser services retain their own practices.

The sideload updater requests GitHub release metadata/assets and compares
versions locally. Its checked code does not send the installed version as a
dedicated GitHub query parameter. Play distribution must use Play's update
path. Opening external pages or sharing/exporting files is an action you
choose and subjects that destination to its own privacy practices.

The current client has no advertising or billing SDK integration, does not
request contacts/calendar/microphone/GPS data, and does not intentionally
infer sensitive personal attributes from content preferences.

## 8. Retention

Furya's private backend maintenance runs daily with these rules:

| Records | Retention rule |
|---|---|
| Statistics device records | 90 days after the last recorded activity |
| Version history | 90 days after the recorded event |
| Private Furya crash-diagnostic copies | 30 days after receipt |
| Historical private bug/feature reports | 90 days after submission |
| Rate-limit records | 7 days |
| Auth security audit records | 90 days, or relevant removal on account erasure |
| Moderation events and resolved content reports | 180 days after the event/resolution |
| Community/Auth profile, links, posts and votes | While the account/discussion is active, until deletion or applicable moderation/retention action; open reports remain for resolution |
| Isolated backups and retired Furya data copies | 30-day expiry; removal at the next scheduled maintenance run |

Older private reports could contain report/reproduction text, app/build/
platform/locale/model/screen information, source-user or guest context, and an
available statistics ID. The old report dialog is no longer an active app
entry point; remaining private records follow the same expiry rule.

Deleted data may temporarily remain in isolated backups until expiry. Those
copies are restricted recovery material, not used as an active service.
Account/data erasure must be re-applied if a recovery copy is restored before
expiry. Scheduled workstation cleanup runs when the workstation is available.

On your device, offline snapshots and read personalized-feed entries have
30-day expiry rules. They are cleaned when the relevant service runs; this is
not a blanket limit for all local files, unread entries or exported downloads.

## 9. Deletion and requests

In builds with the new screen, open **Settings → Storage & Data → Privacy
Controls → Privacy & Account Deletion → Delete community account**. Sign in
with Telegram if necessary and confirm the destructive action. A linked
source account is not required just to delete the Furya Auth account.

The backend erases the Auth account/identities/sessions/refresh state, profile,
source links, roles, individual votes, associated content-report/rate-limit
records, account-owned uploaded files and relevant linked legacy reports.
Authored request/comment text is replaced by a deleted placeholder; other
people's discussion can remain. Relevant moderation records lose the erased
actor/metadata and then follow their expiry rule. This cannot retract copies
others made while a post was public or automatically remove every reference
another person wrote; contact us about such content.

Without the app, or if you cannot sign in, use
[Account and Data Deletion](ACCOUNT_DELETION.md) and email
[Anigx@pushedv.de](mailto:Anigx@pushedv.de). You can also request deletion of
identifiable optional statistics/crash records without deleting your community
account. Statistics IDs are separate from Auth IDs: copy the installation ID
from the privacy screen before removing it if you want us to identify those
records. We may need reasonable proof of ownership and identifying context;
never send passwords, API keys or authentication tokens.

Deletion of a Furya account does not delete a Telegram/source account or local
downloads. Contact the relevant operator for those independently managed
accounts. We normally address privacy requests within 30 days, subject to
necessary identity verification and applicable legal requirements.

## 10. Processing grounds, rights and changes

Furya processes optional telemetry on the basis of your consent, account and
community data to provide the service you request, and proportionate
security/moderation records for protecting that service and addressing abuse.
Where applicable, you may request access, correction, erasure, restriction or
portability, object to applicable processing, withdraw optional consent for
future processing, and complain to a competent data-protection authority.
Use the private contact above. Withdrawal does not undo prior lawful processing.

We date material changes to this notice and update app disclosures/Google Play
Data Safety when practices change. A policy document alone does not install
new app controls; the build-specific availability stated above matters.
