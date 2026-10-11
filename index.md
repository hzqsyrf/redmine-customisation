# Privacy Policy for Redmine Team Customizations

Effective date: October 11, 2026

Redmine Team Customizations is a Chrome and Microsoft Edge extension maintained
by HHI12. Its single purpose is to inject its bundled CSS and JavaScript into
the team's Redmine site to make viewing and managing issues easier.

## Scope

The extension injects code only on the team's internal Redmine site. The
bundled code enhances the Agile board, Issues lists, and issue pages. The
extension does not accept arbitrary code from users or download executable
code from a remote server. It does not monitor browsing on unrelated websites.

This policy describes the packaged browser extension. Development preview
tools are not included in the extension.

## Data handled and why

The injected code handles the following Redmine page data locally to provide
the extension's features:

- **Website and issue content:** Issue identifiers, subjects, descriptions,
  statuses, priorities, estimates, story points, relationships, custom fields,
  links, and other displayed issue information are used to enhance the board,
  lists, and issue sidebar.
- **Personally identifiable information:** Redmine user identifiers, assignee
  names, and profile avatars are used to display assignees and filter cards.
- **Personal communications and form data:** Issue notes, comments, and
  user-entered issue edits, including attachments submitted through the native
  form, are displayed or submitted when the user uses the issue sidebar.
- **Form and request data:** When a user requests an issue edit or priority
  change, the injected code submits the relevant native form fields to
  Redmine. The browser uses the user's existing Redmine session for these
  same-site requests, and native form CSRF tokens are included where required.
  The extension does not ask for or read Redmine passwords, access cookies
  through the browser cookies API, or copy session cookies into extension
  storage.
- **Redmine page URLs and interface activity:** Current board and issue URLs,
  filter selections, and scroll positions are used locally to operate the
  interface and restore it after certain page refreshes. Clicks and other
  interactions trigger the requested interface features, but are not logged
  or sent as activity analytics. This is not a general browsing-history log.
- **Extension preference:** The enable/disable setting determines whether
  customizations are applied.

The extension does not deliberately collect health, financial, payment, or
location information. Issue content is controlled by Redmine users and may
contain information they choose to enter.

## Processing and requests

The extension's bundled code runs in the Redmine page and processes the
information needed for its features in the user's browser. For certain
enhancements, that code retrieves Redmine HTML pages using same-origin
requests. User-requested edits are submitted over HTTPS to the same Redmine
site and remain subject to Redmine's existing permissions and validation.

The extension does not grant additional Redmine access or bypass access controls.
Redmine's own storage, retention, and administration of issue data are governed
by the policies applicable to that service, not by this extension.

## Local storage and retention

- **Enable/disable preference:** Stored in `chrome.storage.local` until changed,
  the extension's stored data is cleared, or the extension is uninstalled.
  The extension does not use Chrome's synchronized storage for this setting.
- **Temporary restoration state:** Board and issue URLs, a timestamp, and
  window and board scroll positions may be stored in the Redmine tab's
  `sessionStorage` before a board refresh. The entry is removed when the
  extension next reads it, and restoration is accepted only when the state
  is less than two minutes old. If it is not read, it remains subject to the
  browser's tab-session storage lifecycle.
- **Runtime data:** Issue and profile information may be cached in browser
  memory while a page is active. The extension does not persist that content
  in its own database or extension storage. Normal browser caching of site
  resources remains subject to browser and Redmine settings.

Disabling the extension stops its customizations but does not delete its
saved enable/disable preference. Uninstalling removes extension-managed local
storage. Temporary restoration state is website session storage, not extension
storage; it can be removed by clearing Redmine's site data in the browser.
Clearing site data may also sign the user out of Redmine.

Removing the extension or clearing browser data does not delete issue changes
already saved to Redmine. Manage those records through Redmine and the
organization responsible for the site.

## Sharing and limited use

The extension has no developer-operated data collection service and does not
send Redmine content, credentials, or usage information to the developer.
It does not include advertising, analytics, or tracking services.

Data is exchanged with the team's Redmine site only as needed for the
extension's features. The extension does not sell user data or share it with
unrelated third parties. It does not use or transfer user data for purposes
unrelated to its single purpose, or to determine creditworthiness or for
lending purposes.

The extension's use of user data is limited to providing its stated
user-facing features.

## Your choices

You can enable or disable customizations from the extension popup or uninstall
the extension at any time. Redmine edits occur through user actions and use
the user's existing permissions. The extension does not automatically upload
issue data to the developer.

If you voluntarily contact support, the recipient receives the information
you include in your message. Do not send passwords, session tokens, or
confidential issue content.

## Changes to this policy

This policy will be updated if the extension's data handling changes. The
effective date above identifies the current version. Chrome Web Store
disclosures will be updated to reflect relevant changes.

## Contact

For privacy questions, contact HHI12 at
[hzqsyrf@gmail.com](mailto:hzqsyrf@gmail.com).
