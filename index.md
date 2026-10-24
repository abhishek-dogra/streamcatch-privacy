---
layout: default
title: StreamCatch Privacy Policy
---
# StreamCatch Privacy Policy

Effective date: October 24, 2026

Developer: Abhishek Dogra  
Contact: [dogra.abhishek113@gmail.com](mailto:dogra.abhishek113@gmail.com)

## 1. Scope

This policy describes how the StreamCatch Chrome extension handles information.
StreamCatch detects media on websites and saves authorized videos using your
browser. It does not require a StreamCatch account or a companion application.

StreamCatch processes detected media and download information on your device.
The extension does not send that information to the developer or operate a
developer-hosted media-processing service. It does make requests to websites
and media providers as described below.

## 2. Information the extension accesses and uses

When enabled on a website, StreamCatch can automatically detect media without
you first clicking Download. Depending on Chrome's site-access settings, this
can occur across HTTP and HTTPS pages and their embedded frames.

To provide detection, previews, video details, and downloads, it accesses:

- **Page and media information:** page URLs and titles, video and source-element
  URLs, poster and social-preview image URLs, and available player information
  such as resolution and duration.
- **Media network information:** request URLs and relevant response metadata,
  such as content type and content length, to identify downloadable media.
  Media URLs can contain query parameters, signed links, or temporary access
  tokens.
- **Preview images:** website-provided images or a small image captured locally
  from a video element when browser security rules permit. This is not a
  screenshot of your entire screen or desktop.
- **Media resources:** manifests, media segments, audio and video tracks, and
  supported non-DRM decryption keys needed to inspect or save selected streams.
- **Download information:** filenames, selected formats and tracks, source
  information needed for retries, download IDs, progress, timing, errors, and
  completion status.
- **Preferences:** your parallel-download limit and selected relative download
  subfolder.

This information is used to display detected videos, inspect available choices,
manage the queue, save files, and provide error recovery. StreamCatch does not
use it to build advertising profiles or a general browsing-history database.
The extension does not include advertising, analytics, tracking SDKs, or
automatic crash-report uploads.

## 3. Network requests and other parties

Local processing does not mean the extension works without network requests.

- Inspecting a detected video can request its manifest and related resources.
  Visible stream cards may be inspected automatically to show video details,
  before you start a download.
- Displaying a website-provided thumbnail can request that image from its host.
  Locally captured preview images do not require an image-server request.
- Downloading requests the selected media and related resources from their
  hosts, which may include third-party content delivery networks. Manifest
  resources may be hosted on domains different from the original page.
- Requests can disclose your IP address, the requested URL and its parameters,
  and ordinary browser request information to the destination. Media fetches
  allow existing site credentials, such as cookies, when Chrome's rules permit.
  StreamCatch does not read or export your cookie database or passwords.
  It does not bypass login requirements, DRM, or other access controls.

Those website, media, and image providers handle requests under their own
privacy policies. Chrome manages browser permissions, storage, downloads, and
extension installation and updates under Google's applicable policies.

StreamCatch does not sell, rent, or transfer detected browsing or media
information to advertising companies, data brokers, or the developer. Its
handling of this information is limited to providing the user-facing media
detection and download features described in this policy.

## 4. Local storage and retention

- **Detected items and page metadata** are kept in Chrome's extension session
  storage. They are cleared for a tab when it closes or its top-level page
  navigates, including supported single-page navigation events. You can also
  clear detected items or remove an individual item from the interface.
  Website activity or a rescan may detect the same media again.
- **Download job records**, including source URLs and retry choices, remain in
  session storage independently of the detected list. Older completed, failed,
  or cancelled records are pruned as new jobs are admitted. Session storage is
  cleared when Chrome ends the browser session or the extension is disabled,
  reloaded, or updated; it is not persistent download history.
- **Preferences** are kept in local extension storage across browser restarts.
  StreamCatch does not use Chrome's synchronized extension storage for them.
  They remain until changed or the extension's local data is removed.
- **Temporary media files** are written to browser-managed private disk storage
  while streams are assembled. StreamCatch attempts to delete them after a job
  finishes, fails, or is cancelled. Crashes, interruptions, or cleanup failures
  may leave files behind; abandoned job files are removed the next time the
  media processor initializes. This is not a promise of immediate deletion or
  secure erasure.
- **Saved downloads** remain in your chosen download location until you delete
  them. Chrome may also retain its own download-history entries. Clearing a
  detected item or uninstalling StreamCatch does not delete downloaded files
  or Chrome's download history.

StreamCatch does not itself synchronize settings or upload local media.
Your operating system, backup software, or a cloud-synchronized download folder
may separately copy files according to your configuration.

## 5. Permissions

StreamCatch uses the following Chrome permissions for its core features:

- **Access to HTTP and HTTPS websites and content scripts:** detect videos and
  page metadata across supported sites and embedded frames, display previews,
  and retrieve media resources.
- **webRequest:** identify media from network response metadata.
- **webNavigation:** clear or refresh detected items when pages change.
- **downloads:** start and monitor downloads, cancel extension-managed jobs,
  and reveal saved files.
- **storage:** retain session information and local preferences.
- **unlimitedStorage:** support large temporary media files without the normal
  storage quota limits. Available disk space still limits processing.
- **offscreen:** perform background media processing while the popup is closed.
- **alarms:** check and maintain download-job status in the background.
- **sidePanel:** provide the dashboard alongside the active website.

Permissions provide capabilities; they do not mean information is sent to the
developer.

## 6. Your choices

You can restrict site access, disable the extension, or uninstall it through
Chrome's extension settings. Restricting access may prevent detection or
downloads on affected sites. You can cancel jobs and clear detected items in
the extension, change saved preferences, and manage downloaded files and
download history separately in Chrome and your file manager.

Uninstalling removes the extension's browser-managed local data, subject to
Chrome's behavior; it does not remove saved downloads or copies in backups.
The developer cannot remotely retrieve or delete data stored only on your
device.

Treat copied media URLs as sensitive: they may contain access tokens. Avoid
sharing them publicly.

## 7. Support communications

If you email support, the developer receives your email address, message, and
any attachments you choose to send. Email providers also process that
correspondence. It is used to respond to your request and troubleshoot issues,
and is retained as needed for support and applicable legal obligations.

Please do not send passwords, cookies, access tokens, private videos, or
unredacted signed media URLs. If you need to request deletion of support
correspondence, contact the email address above.

## 8. Security

Media assembly takes place locally using code bundled with the extension.
Browser security controls apply to extension storage and requests. No software
or storage method can guarantee absolute security. Other software or people
with access to your device, browser profile, backups, or saved files may be
able to access that information. Requests to HTTP-only resources are not
encrypted in transit.

## 9. Changes and contact

This policy may be updated to reflect changes to the extension or its data
handling. The effective date above will identify the latest revision. Material
changes will be described through the extension's release information or
appropriate disclosures.

For privacy questions, contact Abhishek Dogra at
[dogra.abhishek113@gmail.com](mailto:dogra.abhishek113@gmail.com).
