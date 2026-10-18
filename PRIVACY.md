# YLogger app usage information

When enabled in a configured YLogger release, the app reports the signed-in account's display name, an app-specific account reference, a resettable installation identifier, phone manufacturer and model, Android version, app version, and first/last reported activity times to the YLogger usage service.

The purpose is to understand app adoption, supported devices, versions in use, and recent usage. Reports are available only to approved administrators. Account references and names are supplied by the app and do not establish verified identity or attendance.

The service keeps the latest record for each account and installation rather than a history of screens or actions. It does not collect passwords, Yatnam authentication tokens/cookies, precise location, contacts, messages, IMEI, or device serial numbers. Requests are sent only during signed-in foreground use, with reporting paused during Stealth mode. Offline activity is not backfilled.

Installation identifiers reset when the app is uninstalled or its data is cleared. This can leave a previous inactive installation record. Existing service records remain until removed by the project owner; deletion or access requests can be directed to the YLogger project owner through the app's distribution channel.
