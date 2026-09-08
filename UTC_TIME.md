# Understanding UTC

## What is UTC?

**Coordinated Universal Time (UTC)** is the international time standard. In aviation and the military it is often called **Zulu time**. Greenwich Mean Time (GMT) is the same offset as UTC for civil use.

## Why Use UTC?

### Global Coordination
- **No time zone confusion**: When coordinating across multiple time zones, UTC is a single reference point
- **No daylight saving time**: UTC does not observe DST
- **International standard**: Used in aviation, military, weather, and scientific work

### Use Cases
- **Aviation**: Flight plans and air traffic control use UTC
- **Military**: Global operations need synchronized timing
- **Space operations**: NASA and space agencies use UTC
- **Telecommunications**: Network synchronization and logging
- **International business**: Meetings across time zones
- **Emergency services**: Coordinating global response

## How AeroAlarm Uses UTC

### Display
The clock at the top shows the current time in your **reference timezone**. That defaults to UTC. Tap the clock label to pick an airport (IATA). The clock and alarm list then show that city’s local time.

### Alarms
Alarms are stored and scheduled in UTC, even if you entered them in an airport timezone.

- If the reference is **UTC**, setting 14:30 means 14:30 UTC.
- If the reference is **SEA**, setting 07:00 means 07:00 in Seattle, converted to UTC for the alarm.

**Example (reference = UTC):**
- New York (EST, UTC−5): 14:30 UTC = 9:30 AM local
- Tokyo (JST, UTC+9): 14:30 UTC = 11:30 PM local
- London (GMT, UTC+0): 14:30 UTC = 14:30 local

Alarms are **one-time**. After they ring and you stop them, they turn off. Toggle them on again for the next UTC occurrence.

## Converting Between Local Time and UTC

### Quick Reference Table

| Location | Time Zone | UTC Offset | When UTC shows 12:00 |
|----------|-----------|------------|----------------------|
| Los Angeles | PST/PDT | UTC−8/−7 | 4:00 AM / 5:00 AM |
| Denver | MST/MDT | UTC−7/−6 | 5:00 AM / 6:00 AM |
| Chicago | CST/CDT | UTC−6/−5 | 6:00 AM / 7:00 AM |
| New York | EST/EDT | UTC−5/−4 | 7:00 AM / 8:00 AM |
| London | GMT/BST | UTC+0/+1 | 12:00 PM / 1:00 PM |
| Paris | CET/CEST | UTC+1/+2 | 1:00 PM / 2:00 PM |
| Dubai | GST | UTC+4 | 4:00 PM |
| Tokyo | JST | UTC+9 | 9:00 PM |
| Sydney | AEST/AEDT | UTC+10/+11 | 10:00 PM / 11:00 PM |

### Conversion Formula

```
Local Time = UTC + Offset
UTC = Local Time − Offset
```

**Example:**
- You're in New York (UTC−5)
- Current local time is 3:00 PM (15:00)
- UTC = 15:00 − (−5) = 20:00 UTC

### Online Converters
If you need to convert times:
- [timeanddate.com](https://www.timeanddate.com/worldclock/converter.html)
- [worldtimebuddy.com](https://www.worldtimebuddy.com/)
- Search "current UTC time" in any search engine

## Tips for Using AeroAlarm

### Setting Your First Alarm
1. Leave the reference on UTC, or tap the clock label and pick an airport.
2. If you think in local time, either convert to UTC first or select that city’s airport as the reference.
3. UTC entry uses 24-hour format (00:00–23:59). Other reference zones follow your device’s 12-hour or 24-hour setting.

### Common Scenarios

**Morning wake-up (New York, EST)**
- Want 7:00 AM local
- Convert: 7:00 AM EST = 12:00 UTC
- Set the alarm for 12:00 with reference UTC, or pick a New York airport and enter 07:00

**Evening reminder (Tokyo, JST)**
- Want 8:00 PM local
- Convert: 8:00 PM JST = 11:00 UTC
- Set the alarm for 11:00 UTC, or pick a Tokyo airport and enter 20:00

**International meeting**
- Meeting at 15:00 UTC
- Set the alarm for 15:00 with reference UTC

### Verification
Always verify by comparing:

1. The time shown on AeroAlarm’s clock
2. Your local time
3. The offset between them

Most smartphones can show UTC in Clock → World Clock by adding a city in the UTC+0 zone (such as Reykjavik). You can also ask Siri: “What's UTC in AeroAlarm.”

## 24-Hour Time Format

UTC uses 24-hour format:

| 12-Hour | 24-Hour |
|---------|---------|
| 12:00 AM | 00:00 |
| 1:00 AM | 01:00 |
| 6:00 AM | 06:00 |
| 12:00 PM | 12:00 |
| 1:00 PM | 13:00 |
| 6:00 PM | 18:00 |
| 11:00 PM | 23:00 |
| 11:59 PM | 23:59 |

## Why Not Just Use Local Time?

Local time works for personal routines. UTC is useful when:

1. **Traveling**: The UTC alarm stays the same across time zones
2. **Remote teams**: No confusion about “9 AM your time or mine?”
3. **Documentation**: Timestamps that do not shift with DST
4. **Precision**: Fewer DST and time-zone mistakes

AeroAlarm’s airport reference is a display and entry aid. The scheduled wake-up is still a UTC time.

## Additional Resources

- [What is UTC?](https://en.wikipedia.org/wiki/Coordinated_Universal_Time)
- [Time Zone Map](https://www.timeanddate.com/time/map/)
- [UTC Time Now](https://time.is/UTC)

## Questions?

Email [support@northernhangar.com](mailto:support@northernhangar.com) or [open a GitHub Issue](https://github.com/nchodge/AeroAlarm_docs/issues/new/choose).
