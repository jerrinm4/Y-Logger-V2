# YLogger information and shared dates

YLogger keeps attendance-service credentials and cached profiles on the phone.
Passwords, attendance-service tokens and cookies, contact details, blood group,
and complete profiles are not sent to the shared-dates service.

Configured releases send an app-specific account reference, display name,
resettable installation identifier, phone manufacturer/model, Android/app
versions, and first/last activity times to the private usage service. These
reports help the owner understand adoption and supported devices; they are
visible only to authorized administrators and do not verify identity or attendance.
Usage reports run during signed-in foreground use, pause in Stealth, and do not
backfill offline activity.

## Shared birthdays and work anniversaries

Administrators independently enable Read and Write for each phone/account,
allowing Off, Read only, Write only, or both.
New installations default to Off. Approved phones using the same attendance
service share dates automatically, without a company selection or setup step.
Access requires the installation credential and administrator permission; an
account reference alone does not grant access.

Authorized reads download employee identifiers, minimal display names,
birthdays (including a year only when known), joining dates and work-anniversary
dates. Write-enabled phones can contribute missing dates already stored on the
phone and share deliberate corrections. Automatic imports preserve existing
shared values. Inferred joining years are not uploaded as confirmed dates.
Attendance, leave balances, contact information and full profiles are excluded.

Dates remain cached for offline use. Shared records remain until an
administrator corrects or removes them. Removing a shared entry propagates on
the next successful synchronization; original-service data and personal local
edits remain on the phone. Revoking Read blocks further downloads and clears
downloaded-only dates when the phone next refreshes its access status. Revoking
Write blocks further contributions without deleting original or local dates.
An offline phone may retain a previously downloaded copy until it reconnects.

## Storage, control and requests

Installation credentials are stored separately from attendance credentials.
Uninstalling or clearing app data resets the installation identity and its
shared-date access. Updates and ordinary sign-out retain the installation;
signed-out phones do not synchronize dates. Automatic sync pauses in the
background and during Stealth.

The service does not collect precise location, phone contacts, messages, IMEI,
or device serial numbers. Shared records are available only to authorized phones using the same
attendance service, or to approved administrators. Existing usage records remain
until removed by the owner. Access, correction, or deletion requests can be
directed to the YLogger project owner through the app's distribution channel.
