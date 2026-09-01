# AeroAlarm Support

AeroAlarm is a UTC (Zulu time) alarm clock for iOS and Android. All times in the app are in 24-hour UTC—never local time.

## Get Help

**Email:** [support@northernhangar.com](mailto:support@northernhangar.com)

**Bug reports and questions:** [Open a GitHub Issue](https://github.com/nchodge/AeroAlarm_docs/issues/new/choose)

Please include:

- Device model and OS version
- AeroAlarm version (Settings or App Store listing)
- What you expected vs. what happened
- For alarm issues: the UTC time you set and your local time zone

**Privacy questions:** see [Privacy Policy](PRIVACY.md)

## Quick Start

1. Open AeroAlarm—the large clock at the top shows current **UTC** time.
2. Tap **+** to add an alarm in UTC (00:00–23:59).
3. Toggle an alarm on or off with the switch.
4. Long-press an alarm to delete it.
5. When an alarm rings: snooze for 5 minutes or slide to stop.

New to Zulu time? Read [Understanding Zulu Time](ZULU_TIME.md).

## Troubleshooting

### Alarm did not ring

1. **Use a physical device.** Alarms are unreliable or unavailable in simulators/emulators.
2. **Set the alarm at least 15 seconds ahead** of the current UTC time shown in the app.
3. **Enable wake-up alarm permissions** in the app (Settings gear → Wake-up Alarms).
4. **iOS:** Allow **Alarms** under **Settings → Notifications → AeroAlarm**.  
   Note: Alarms is not on the main Settings → AeroAlarm page.
5. **Android:** Allow **exact alarms** and **full-screen / lock-screen alarms** when prompted.
6. **Focus / Do Not Disturb:** AeroAlarm is built to ring through these modes, but OS settings can still block alerts—check system notification settings if problems persist.

### Snooze or stop did not work

- Use the in-app full-screen alarm view: **Snooze (5 min)** or **slide to stop**.
- Return to the app if you dismissed the alarm from the system UI—the app reconciles alarm state when opened.

### Wrong time fired

Alarms always use **UTC**, not your phone’s local time zone.

Example: 14:30 in AeroAlarm = 14:30 Zulu = 9:30 AM Eastern (UTC−5), not 2:30 PM local.

See [ZULU_TIME.md](ZULU_TIME.md) for conversion help.

### Haptic before sound

In **Settings → Haptic for 1 min, then sound**, you can vibrate for about one minute at alarm time, then play sound. Turning this on re-schedules enabled alarms.

## Permissions Summary

| Platform | What to allow |
|----------|----------------|
| iOS | Alarms (AlarmKit) via in-app prompt or Settings → Notifications → AeroAlarm |
| Android | Exact alarms; full-screen intent for lock-screen alarms |

## Links

- [README](README.md) — features and overview
- [Privacy Policy](PRIVACY.md)
- [Zulu Time Guide](ZULU_TIME.md)

## App Store URLs

Use these links in App Store Connect:

| Field | URL |
|-------|-----|
| Support URL | `https://github.com/nchodge/AeroAlarm_docs/blob/main/SUPPORT.md` |
| Privacy Policy URL | `https://github.com/nchodge/AeroAlarm_docs/blob/main/PRIVACY.md` |
| Marketing URL (optional) | `https://github.com/nchodge/AeroAlarm_docs` |
