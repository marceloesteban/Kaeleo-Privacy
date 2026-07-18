# Kaeleo Privacy Policy

Effective date: 19 July 2026
Contact: marceloluengoquinones@gmail.com

This policy describes the data Kaeleo stores locally, syncs through your private
iCloud account, and sends to Cloud AI only when you explicitly approve a
feature. The App Store privacy answers and the submitted binary are intended to
match this policy.

## What Kaeleo stores

Projects, tasks, notes, reminders, recordings, transcripts, attachments,
posture calibration, and 3D scan data are stored locally so Kaeleo can provide
its core features. When iCloud sync is available, workspace records and
attachments sync through the user's private CloudKit container. This includes
the latitude/longitude and place label selected for an arrival/departure
reminder, plus 3D scan model attachments and scan metadata. Profile name, role,
and preferences use Apple's private iCloud key-value store.

Location is used only for user-created arrival/departure reminders and is never
tracked continuously in the background. Apple Health data is accessed only for
Focus Wellness and remains in HealthKit and transient in-memory processing;
Kaeleo does not store HealthKit samples or HealthKit-derived personal health
data in app-managed iCloud.

## Permissions and device data

Kaeleo requests protected access only when a related feature is started:

- Camera: text/document scanning, note photos and videos, LiDAR room or object
  capture on supported hardware, and optional on-device TrueDepth posture
  alignment.
- Microphone and speech recognition: note recordings, dictation, and Luna Live
  Voice.
- Motion and AirPods route data: optional posture cues.
- Location: a user-selected arrival/departure reminder region, not continuous
  tracking.
- Files and Photos: content selected through Apple's system pickers.

TrueDepth facial/depth alignment is transient, processed on the device, and is
not stored, transmitted, or used to identify you. You can decline any permission
and continue to use unrelated local features.

HealthKit, AirPods motion, reminder location, LiDAR meshes, and TrueDepth
alignment are never sent to Kaeleo's Cloud AI service.
Reminder coordinates and user-captured 3D scan model data may sync through the
private CloudKit workspace when iCloud sync is enabled.

## Optional Cloud AI

Kaeleo does not send content to Cloud AI unless you explicitly allow the
specific feature immediately before its first transfer. The permissions are:

- **Luna text and files:** prompts, selected workspace context, conversation
  context, and selected attachments.
- **Luna Live Voice:** microphone audio, speech transcripts, and selected Luna
  context while a Live session is active.
- **Meeting analysis:** a selected recording transcript, note/project context,
  and selected document attachments.

Kaeleo's authenticated Cloudflare service forwards permitted requests to OpenAI
to produce the requested result. OpenAI API data is not used to train models by
default. OpenAI abuse-monitoring records may be retained for up to 30 days.
Background meeting responses use OpenAI's background processing and may be
retained under OpenAI's API retention policy; Kaeleo's authenticated poll token
expires after about nine minutes and Kaeleo does not retain the meeting
transcript in its own database.

Luna web-search queries are sent only to service the selected request with
OpenAI's no-storage request setting. Kaeleo does not keep a search-history
database or use searches for advertising or profiling.

Kaeleo does not send Apple Health data, facial/depth geometry, continuous
location, or private 3D scan meshes to Cloud AI. Kaeleo does not use this data
for advertising, tracking, marketing, or profiling.

## Security and identifiers

Short-lived Cloud AI session credentials and App Attest identifiers are stored
in the device Keychain. App Attest helps the service verify the installation; it
is not an advertising identifier. Requests use HTTPS/WSS. Kaeleo does not use
the App Tracking Transparency framework because it does not track users.

## Your choices and deletion

You can decline or revoke each Cloud AI permission at **Settings → Privacy
Choices**. Revocation stops future transfers. It cannot erase provider security
logs that were already created.

You can delete projects, notes, reminders, recordings, attachments, and scans
from Kaeleo. Deleted workspace items move to **Recently Deleted** for the
retention period shown in the app and are then purged. Deleting the app removes
local data, while private iCloud copies are managed through your Apple account
and iCloud controls. Provider security records follow the provider retention
rules described above and cannot be erased by Kaeleo.

## Third-party services

Apple provides iCloud/CloudKit, HealthKit, MusicKit, and system permission
services under Apple's terms and privacy controls. Cloudflare and OpenAI process
only feature data you authorize and apply their own security, retention, and
privacy terms. Review [Cloudflare's Privacy Policy](https://www.cloudflare.com/policies/privacy/)
and [OpenAI's API data controls](https://developers.openai.com/api/docs/guides/your-data)
for the provider rules that apply alongside this policy.

## Contact

For privacy questions, deletion requests, or support, contact:

**Marcelo Luengo**
**marceloluengoquinones@gmail.com**
