# NotebookRemainder

**NotebookRemainder** is an Android planner built around missions,
events, reminders, alarms, and a private encrypted notebook.

The goal is to keep everyday planning simple while still supporting the
things that are easy to miss: deadlines, classes, recurring events,
wake-up alarms, attendance, holidays, and important private notes.

## Main features

### Missions

Create missions with deadlines, categories, workload, importance, notes,
links, recurrence, and reminder settings.

-   Upcoming and overdue missions
-   Quick add
-   Started / Done status
-   Recurring missions
-   Search and filters
-   Calendar integration
-   Rescheduling
-   Configurable reminder timing

### Events and classes

Events live alongside missions and can include a start/end time,
category, online or physical location, meeting link, time zone,
reminders, wake-up alarm, optional attendance tracking, and repeating
schedules.

Repeating events support common schedules such as daily, weekdays,
weekly, and monthly, plus custom intervals, end dates, occurrence
counts, selected exact dates, and skipped/rescheduled occurrences.

### Calendar

Day, Week, and Month views combine:

-   Mission deadlines
-   Timed events
-   Holidays
-   Today highlighting
-   Current-time information
-   Direct Mission / Event creation from a selected date

The app can display public holidays for supported countries plus
optional Jewish, Christian, and Islamic observances. Holiday coverage
depends on the available sources and is intended as planning information
rather than an authoritative religious calendar.

### Today / Upcoming

The main screen provides a quick view of what matters now, including the
current or next event, missions due today, overdue missions, quick
Start/Done actions, future events, and a Tomorrow preview.

### Reminders

Mission and event reminders can be scheduled at different intervals
before their deadline or start time. Reminder behavior can become more
persistent as an item becomes urgent.

### Wake-up alarms

Events can automatically create wake-up alarms based on how early you
need to wake. Multiple events on the same day can be consolidated around
the earliest required wake time.

Wake-up alarms currently support:

-   Gentle, Normal, and Heavy intensity
-   Escalation after repeated snoozes
-   Unlimited snooze
-   Random or fixed challenge behavior
-   Math challenges
-   Memory challenges
-   Typing challenges
-   Configurable challenge difficulty

Standalone alarms can also be created independently of events.

### Daily summary

A daily overview can include the day's events, missions, and holidays.
When an event wake-up alarm is used, the summary can appear after the
alarm is dismissed instead of producing a duplicate morning
notification.

### Attendance

Attendance tracking is optional and off by default. Tracked event
occurrences can be marked Attended or Missed, allowing the app to
calculate attendance information from recorded occurrences.

### Time zones

Events retain their original time zone. When it differs from the
device's current zone, the app can also display the corresponding local
time. This is useful for online classes, travel, and schedules created
for another country.

### Sounds

Mission reminders, event reminders, and wake-up alarms can use separate
sounds. You can choose from the phone's available notification/alarm
sounds or select an audio file from the device.

## Private vault

NotebookRemainder also contains a hidden private notebook/password
vault, separated from the normal planner interface and opened through a
hidden action in Settings.

The vault includes:

-   Master-password protection
-   Encrypted note storage
-   Password hint support
-   Screenshot protection while the vault is open
-   Clipboard protections
-   Automatic locking when leaving the app
-   Encrypted backup and restore
-   Encrypted cross-device synchronization

The master password itself is not uploaded as part of vault
synchronization.

## Sync

Optional account-based synchronization can keep planner information and
the encrypted vault available across devices.

Synced planner data includes missions, categories, events, standalone
alarms, and settings.

The synchronization system is still being hardened for more complex
cases such as simultaneous edits on multiple devices and account
switching. Important information should not rely on sync as its only
backup.

## Updates

NotebookRemainder can check its GitHub releases for newer APK versions.
It can detect an update, download the APK, show download progress/state,
and notify when installation is ready.

Android still requires the user to approve APK installation. The app
does not silently replace itself.

## Privacy

NotebookRemainder is designed as a personal-use planner. Private-vault
contents are encrypted before synchronization. Planner synchronization
requires an account and network access. Holiday data and update checks
may also require internet access.

## Technology

-   Android
-   Kotlin
-   Jetpack Compose / Material 3
-   Minimum Android SDK 26
-   Target/compile SDK 37
-   Android scheduling and notification APIs
-   Supabase-backed optional synchronization
-   GitHub Releases based application updates

## Development status

NotebookRemainder is under active development. Current priorities
include:

-   Stronger wake-up challenges and mini-games
-   Better heavy-sleeper alarm behavior
-   Calendar and event usability
-   Time-zone handling
-   Cross-device sync reliability
-   General UI cleanup and simplification

## Installation

NotebookRemainder is currently distributed as an Android APK through
GitHub Releases.

To update an existing installation, install a newer APK signed with the
same application signing key. Android may scan each downloaded APK and
will ask for confirmation before installing an update.

------------------------------------------------------------------------

NotebookRemainder is designed to make important things difficult to miss
without turning everyday planning into a complicated system.
