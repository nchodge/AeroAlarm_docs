# AeroAlarm Support

AeroAlarm is a UTC alarm clock for iOS and Android. Alarms are stored and fire in **UTC**. You can display and enter times in UTC or in an airport reference timezone.

## Get Help

**Email:** [support@northernhangar.com](mailto:support@northernhangar.com)

**Bug reports and questions:** [Open a GitHub Issue](https://github.com/nchodge/AeroAlarm_docs/issues/new/choose)

Please include:

- Device model and OS version (iOS 26+ is required for iPhone wake-up alarms)
- AeroAlarm version (Settings or App Store listing)
- What you expected vs. what happened
- For alarm issues: the time you set, the reference timezone shown in the app (for example UTC or SEA), and your local time zone

**Privacy questions:** see [Privacy Policy](PRIVACY.md)

## Quick Start

1. Open AeroAlarm. The large clock at the top shows the current **reference timezone** (UTC by default).
2. Tap **UTC TIME** (or the airport code) to pick a reference airport. Clock and alarm entry follow that zone; alarms still fire at a UTC instant.
3. Tap **+** to add a one-time alarm. Enter the time in the reference zone, then **Add Alarm**.
4. Toggle an alarm on or off with the switch.
5. Tap an alarm time to edit it. Swipe left to delete it.
6. When an alarm rings: snooze for 5 minutes or stop it. After you stop it, the alarm turns off (one-time).

New to UTC? Read [Understanding UTC](UTC_TIME.md).

## Troubleshooting

### Alarm did not ring

1. **Use a physical device.** Alarms are unreliable or unavailable in simulators/emulators.
2. **Set the alarm at least 15 seconds ahead** of the current time shown in the app.
3. **Enable wake-up alarm permissions** in the app (Settings gear → Wake-up Alarms).
4. **iOS 26 or later** is required. Wake-up alarms use Apple AlarmKit, which can ring through Focus, Silent Mode, and the lock screen.
5. **iOS:** Allow **Alarms** under **Settings → Apps → AeroAlarm**.  
   If Alarms is missing, open AeroAlarm → Settings → Wake-up Alarms and tap **Request alarm permission**.
6. **Android:** Allow **Alarms & reminders** (exact alarms) and **full-screen / lock-screen alarms**. On Samsung, Xiaomi, Oppo, and Vivo, also turn off battery optimization for AeroAlarm.
7. **One-time alarms do not repeat.** After an alarm rings and you stop it, it stays in the list but is turned off. Toggle it on again for the next UTC occurrence.

### Snooze or stop did not work

- **iOS:** Use the system AlarmKit stop/snooze controls. Returning to AeroAlarm also reconciles alarm state.
- **Android:** Use the in-app full-screen alarm view: **Snooze (5 min)** or **slide to stop**.
- If you dismissed the alarm from the system UI, open AeroAlarm so it can update the alarm list.

### Wrong time fired

Alarms always fire in **UTC**, even if the clock shows an airport timezone.

Example: with the reference set to UTC, 14:30 in AeroAlarm = 14:30 UTC = 9:30 AM Eastern (UTC−5), not 2:30 PM local.

If the clock shows an airport (for example SEA), you are entering that city’s wall-clock time. AeroAlarm converts it to UTC for scheduling. After a daylight-saving change, the same UTC alarm can show a different local time in that city.

See [UTC_TIME.md](UTC_TIME.md) for conversion help.

### Haptic before sound

In **Settings → Haptic for 1 min, then sound**, you can vibrate for about one minute at alarm time, then play sound. Turning this on re-schedules enabled alarms.

## Siri and Shortcuts (iOS)

AeroAlarm includes App Shortcuts. Examples:

| Ask Siri | What it does |
|----------|----------------|
| “Set 14:30 in AeroAlarm” | Set a UTC alarm |
| “What's UTC in AeroAlarm” | Speak the current UTC time |
| “Set reference timezone in AeroAlarm” | Change the airport reference (IATA code) |
| “Snooze AeroAlarm” | Snooze the ringing alarm |
| “Stop AeroAlarm” | Stop the ringing alarm |

Siri scheduling still needs AlarmKit permission. Open AeroAlarm and allow Alarms before using Siri to set a wake-up.

## Permissions Summary

| Platform | What to allow |
|----------|----------------|
| iOS 26+ | Alarms (AlarmKit) via in-app prompt or Settings → Apps → AeroAlarm |
| Android | Alarms & reminders (exact alarms); full-screen notifications for lock-screen alarms |

## Links

- [README](README.md) — features and overview
- [Privacy Policy](PRIVACY.md)
- [UTC Guide](UTC_TIME.md)

## App Store URLs

Use these links in App Store Connect:

| Field | URL |
|-------|-----|
| Support URL | `https://github.com/nchodge/AeroAlarm_docs/blob/main/SUPPORT.md` |
| Privacy Policy URL | `https://github.com/nchodge/AeroAlarm_docs/blob/main/PRIVACY.md` |
| Marketing URL (optional) | `https://github.com/nchodge/AeroAlarm_docs` |
