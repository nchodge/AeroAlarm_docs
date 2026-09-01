# AeroAlarm

**UTC & Zulu time alarms for iOS and Android.**

AeroAlarm is a focused alarm clock that displays and schedules everything in Zulu time (UTC). Set a time once in 24-hour UTC—no time zone math, no daylight saving surprises. Built for pilots, crews, travelers, and anyone who thinks in Zulu.

## Features

- **Live UTC clock** — large Zulu time display, updated every second
- **UTC alarms** — set alarms in 24-hour Zulu time (00:00–23:59)
- **Native wake-up alarms** — rings through iOS Focus and Android Do Not Disturb when permitted
- **Lock-screen alerts** — full-screen alarm view with snooze and slide-to-stop
- **Snooze** — 5-minute snooze with countdown
- **Optional haptic lead** — vibrate for about one minute, then play sound
- **Simple UI** — add, toggle, and long-press to delete alarms; no account required

## Support

- **Email:** [support@northernhangar.com](mailto:support@northernhangar.com)
- **Help & troubleshooting:** [SUPPORT.md](SUPPORT.md)
- **Bug reports & questions:** [GitHub Issues](https://github.com/nchodge/AeroAlarm_docs/issues/new/choose)
- **Zulu time guide:** [ZULU_TIME.md](ZULU_TIME.md)
- **Privacy policy:** [PRIVACY.md](PRIVACY.md)

## Screenshots

The app features:

- Upper third: large UTC clock with date
- Upper corners: Settings and Add (+) buttons
- Lower section: scrollable alarm list with UTC times and toggles

## Usage

1. **View current time** — UTC is always shown at the top.
2. **Add an alarm** — tap **+**, enter hours (00–23) and minutes (00–59) in UTC, then **Add Alarm**.
3. **Toggle alarms** — use the switch on each row.
4. **Delete an alarm** — long-press the alarm, then confirm delete.
5. **When ringing** — snooze for 5 minutes or slide to stop.

Alarms must be set at least 15 seconds ahead of the current UTC time. Use a physical device for reliable alarm testing.

## Permissions

AeroAlarm needs alarm permissions so wake-ups can ring on a locked phone.

### iOS

- **Alarms (AlarmKit):** schedule wake-up alarms that can alert through Focus and the lock screen  
  Enable under **Settings → Notifications → AeroAlarm → Alarms**

### Android

- **Exact alarms:** precise UTC scheduling
- **Full-screen intent:** alarm on lock screen
- **Vibration:** haptic alerts

See [SUPPORT.md](SUPPORT.md) for step-by-step troubleshooting.

## Privacy

AeroAlarm does not collect or transmit personal data. Alarm settings are stored on your device only.  
Full details: [PRIVACY.md](PRIVACY.md)
