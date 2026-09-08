# AeroAlarm

**UTC alarms for iOS and Android.**

AeroAlarm is a focused alarm clock that stores and fires every alarm in UTC. Display and enter times in UTC, or in an airport reference timezone. Built for pilots, crews, travelers, and anyone who schedules in UTC.

## Features

- **Live clock** — large clock for UTC or a selected airport timezone, updated every second
- **Reference timezone** — tap the clock label to search airports by IATA, city, or country
- **UTC alarms** — times are stored as UTC; one-time alarms that turn off after they stop
- **Native wake-up alarms** — iOS AlarmKit (iOS 26+) rings through Focus, Silent Mode, and the lock screen; Android uses exact alarms and full-screen lock-screen alerts
- **Snooze** — 5-minute snooze
- **Siri & Shortcuts (iOS)** — set a UTC alarm, show UTC time, change reference timezone, snooze, or stop
- **Optional haptic lead** — vibrate for about one minute, then play sound
- **Simple UI** — add, edit, toggle, and swipe to delete; no account required

## Support

- **Email:** [support@northernhangar.com](mailto:support@northernhangar.com)
- **Help & troubleshooting:** [SUPPORT.md](SUPPORT.md)
- **Bug reports & questions:** [GitHub Issues](https://github.com/nchodge/AeroAlarm_docs/issues/new/choose)
- **UTC guide:** [UTC_TIME.md](UTC_TIME.md)
- **Privacy policy:** [PRIVACY.md](PRIVACY.md)

## Screenshots

The app features:

- Header: Settings, live clock with date, and Add (+)
- Clock label: tap to change the reference timezone (UTC or airport)
- Alarm list: times in the reference zone, labeled as one-time, with on/off switches

## Usage

1. **View current time** — the clock shows the selected reference timezone (UTC by default).
2. **Change reference timezone** — tap the clock label, then search by IATA, city, or country.
3. **Add an alarm** — tap **+**, enter hours and minutes in the reference zone, then **Add Alarm**.
4. **Edit an alarm** — tap the alarm time.
5. **Toggle alarms** — use the switch on each row.
6. **Delete an alarm** — swipe left, then confirm.
7. **When ringing** — snooze for 5 minutes or stop. The alarm then turns off (one-time).

Alarms must be set at least 15 seconds ahead of the current reference time. Use a physical device for reliable alarm testing. iPhone wake-up alarms require iOS 26 or later.

## Permissions

AeroAlarm needs alarm permissions so wake-ups can ring on a locked phone.

### iOS (26+)

- **Alarms (AlarmKit):** schedule wake-up alarms that can alert through Focus, Silent Mode, and the lock screen  
  Enable in AeroAlarm → Settings → Wake-up Alarms, or **Settings → Apps → AeroAlarm → Alarms**

### Android

- **Alarms & reminders (exact alarms):** precise UTC scheduling
- **Full-screen notifications:** alarm on lock screen
- **Vibration:** haptic alerts

See [SUPPORT.md](SUPPORT.md) for step-by-step troubleshooting.

## Privacy

AeroAlarm does not collect or transmit personal data. Alarm settings stay on your device.  
Full details: [PRIVACY.md](PRIVACY.md)
