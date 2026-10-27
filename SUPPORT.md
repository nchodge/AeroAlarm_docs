# AeroAlarm Support

AeroAlarm is a UTC alarm clock for iOS and Android. Alarms are stored and fire in **UTC**. You can display and enter times in UTC or in an airport reference timezone.

The iPhone app requires **iOS 26 or later**. Wake-up alarms use Apple AlarmKit, which can ring through Focus, Silent Mode, and the lock screen.

## Get Help

**Email:** [support@northernhangar.com](mailto:support@northernhangar.com)

**Bug reports and questions:** [Open a GitHub Issue](https://github.com/nchodge/AeroAlarm_docs/issues/new/choose)

Please include:

- Device model and OS version (iOS 26 or later is required on iPhone)
- AeroAlarm version from the App Store or Play Store listing, or from the system app screen (**Settings → Apps → AeroAlarm** on iPhone, App info on Android). The in-app Settings sheet does not show the version.
- What you expected vs. what happened
- For alarm issues: the time you set, the reference timezone on the clock (for example UTC or SEA), whether the phone uses 12-hour or 24-hour time, and your local time zone

**Privacy questions:** see [Privacy Policy](PRIVACY.md)

## Quick Start

1. Open AeroAlarm. The large clock at the top shows the current **reference timezone** (UTC by default).
2. Tap the clock label (**UTC TIME**, **SEA TIME**, and so on) to open **Reference Timezone**. Search by city or IATA code. UTC stays at the top. Recently used airports are listed under Recent.
3. The clock and new alarms follow that zone. Alarms are still stored and fired as a UTC instant.
   - **UTC** is always 24-hour (00:00–23:59).
   - An airport reference follows the phone’s 12-hour or 24-hour setting. In 12-hour mode, enter the hour and minutes, then choose **AM** or **PM**.
4. Tap **+** to add a one-time alarm. Enter the time in the reference zone, then **Add Alarm**. Set it at least 15 seconds ahead of the clock.
5. Toggle an alarm on or off with the switch. Each row is labeled with the reference and **One-time** (for example `UTC · One-time`).
6. Tap an alarm time to edit it, then **Save**. Swipe left and tap **Delete** to remove it.
7. When an alarm rings:
   - **iPhone:** use the system AlarmKit **Snooze** or stop controls. Snooze is 5 minutes.
   - **Android:** use the full-screen alarm: **Snooze (5 min)** or **slide to stop**.
8. One-time alarms do not repeat. After one fires and is stopped, it stays in the list with the switch off. If you stopped it outside the app, open AeroAlarm so the list can update. Turn the switch on again to schedule the next occurrence of that UTC time.

New to UTC? Read [Understanding UTC](UTC_TIME.md).

## Lock screen countdown (iPhone)

While an alarm is on, iPhone shows a Live Activity on the Lock Screen and in the Dynamic Island. It shows:

- the current reference time, in 24-hour form
- the alarm time
- a countdown until it rings

During snooze, the countdown covers the 5-minute snooze window.

The alarm still rings if Live Activities are off. To show the countdown, turn on **Settings → Apps → AeroAlarm → Live Activities**.

Android does not use this Live Activity. When the alarm is due, Android opens the full-screen alarm in AeroAlarm.

## Troubleshooting

### Alarm did not ring

1. **Use a physical device.** Alarms are unreliable or unavailable in simulators and emulators.
2. **Set the alarm at least 15 seconds ahead** of the current time shown in the app.
3. **Enable wake-up alarm permissions** in the app (Settings gear → **Wake-up Alarms**).
4. **iOS 26 or later** is required. The iPhone app will not run on earlier versions.
5. **iPhone:** Allow **Alarms** under **Settings → Apps → AeroAlarm**.  
   If Alarms is missing, open AeroAlarm → Settings → Wake-up Alarms and tap **Request alarm permission**.
6. **Android:** Allow **Alarms & reminders** (exact alarms) and lock-screen alarms. In AeroAlarm → Settings → Wake-up Alarms, use **Open alarm settings** and **Allow lock-screen alarms** when those buttons are shown. On Samsung, Xiaomi, Oppo, and Vivo, also turn off battery optimization for AeroAlarm.
7. **One-time alarms do not repeat.** After an alarm fires and you stop it, it stays in the list but is turned off. Toggle it on again for the next UTC occurrence.

### Countdown did not appear (iPhone)

- Turn on **Live Activities** for AeroAlarm under **Settings → Apps → AeroAlarm**.
- The countdown is only for an alarm that is still on and still upcoming. A one-time alarm that has already fired will not show one.
- Live Activities are the countdown only. Turning them off does not stop the alarm from ringing.

### Snooze or stop did not work

- **iPhone:** Use the system AlarmKit stop and snooze controls. Returning to AeroAlarm also updates the alarm list.
- **Android:** Use the in-app full-screen alarm: **Snooze (5 min)** or **slide to stop**.
- If you dismissed the alarm from the system UI, open AeroAlarm so it can turn that one-time alarm off.

### Wrong time fired

Alarms always fire at a **UTC** instant, even when the clock shows an airport timezone.

With the reference set to UTC, 14:30 in AeroAlarm is 14:30 UTC. That is 9:30 AM Eastern Standard Time (UTC−5), not 2:30 PM local.

If the clock shows an airport (for example SEA), you are entering that city’s wall-clock time. AeroAlarm converts it to UTC for scheduling. After a daylight-saving change, the same UTC alarm can show a different local time in that city.

If the phone is set to 12-hour time and the reference is an airport, the in-app clock and alarm list use AM/PM. UTC stays 24-hour either way. The iPhone lock-screen countdown clock is 24-hour even when the in-app airport clock shows AM/PM. Compare the alarm time on the row, not only the live clock on the Lock Screen.

See [UTC_TIME.md](UTC_TIME.md) for conversion help.

### Haptic before sound

In **Settings → Haptic for 1 min, then sound**, AeroAlarm vibrates for about one minute at the alarm time, then plays sound. Off rings with sound immediately. Turning this on or off re-schedules enabled alarms.

## Siri and Shortcuts (iOS)

AeroAlarm includes App Shortcuts. Examples:

| Ask Siri | What it does |
|----------|----------------|
| “Set 14:30 in AeroAlarm” | Set a **UTC** alarm (always UTC, even if the clock shows an airport) |
| “What's UTC in AeroAlarm” | Speak the current UTC time |
| “Set reference timezone in AeroAlarm” | Change the airport reference (IATA code) |
| “Snooze AeroAlarm” | Snooze the ringing alarm for 5 minutes |
| “Stop AeroAlarm” | Stop the ringing alarm |

Siri scheduling still needs AlarmKit permission. Open AeroAlarm and allow Alarms before using Siri to set a wake-up.

## Permissions Summary

| Platform | What to allow |
|----------|----------------|
| iOS 26+ | **Alarms** (AlarmKit), from the in-app prompt or **Settings → Apps → AeroAlarm** |
| iOS | **Live Activities** (optional) for the Lock Screen and Dynamic Island countdown |
| Android | **Alarms & reminders** (exact alarms), and full-screen / lock-screen alarms |

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
