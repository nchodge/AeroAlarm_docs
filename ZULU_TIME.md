# Understanding Zulu Time (UTC)

## What is Zulu Time?

**Zulu Time** is the military and aviation term for **Coordinated Universal Time (UTC)**, which is also known as **Greenwich Mean Time (GMT)**. The letter "Z" in the NATO phonetic alphabet is pronounced "Zulu."

## Why Use Zulu Time?

### Global Coordination
- **No Time Zone Confusion**: When coordinating across multiple time zones, UTC provides a single reference point
- **No Daylight Saving Time**: UTC does not observe DST, eliminating seasonal confusion
- **International Standard**: Used universally in aviation, military, weather, and scientific applications

### Use Cases
- **Aviation**: All flight plans and air traffic control use Zulu time
- **Military**: Global operations require synchronized timing
- **Space Operations**: NASA and space agencies use UTC exclusively
- **Telecommunications**: Network synchronization and logging
- **International Business**: Conference calls across time zones
- **Emergency Services**: Coordinating global response efforts

## How This App Uses Zulu Time

### Display
The clock at the top of the app always shows the current UTC time, updating every second. This is calculated using JavaScript's UTC methods, ensuring accuracy regardless of your device's local time zone setting.

### Alarms
When you set an alarm for "14:30", it will trigger at 14:30 UTC (2:30 PM Zulu time), regardless of your local time zone.

**Example:**
- If you're in New York (EST, UTC-5):
  - Setting alarm for 14:30 UTC = 9:30 AM local time
- If you're in Tokyo (JST, UTC+9):
  - Setting alarm for 14:30 UTC = 11:30 PM local time
- If you're in London (GMT, UTC+0):
  - Setting alarm for 14:30 UTC = 14:30 local time

## Converting Between Local Time and Zulu Time

### Quick Reference Table

| Location | Time Zone | UTC Offset | When Zulu shows 12:00 |
|----------|-----------|------------|----------------------|
| Los Angeles | PST/PDT | UTC-8/-7 | 4:00 AM / 5:00 AM |
| Denver | MST/MDT | UTC-7/-6 | 5:00 AM / 6:00 AM |
| Chicago | CST/CDT | UTC-6/-5 | 6:00 AM / 7:00 AM |
| New York | EST/EDT | UTC-5/-4 | 7:00 AM / 8:00 AM |
| London | GMT/BST | UTC+0/+1 | 12:00 PM / 1:00 PM |
| Paris | CET/CEST | UTC+1/+2 | 1:00 PM / 2:00 PM |
| Dubai | GST | UTC+4 | 4:00 PM |
| Tokyo | JST | UTC+9 | 9:00 PM |
| Sydney | AEST/AEDT | UTC+10/+11 | 10:00 PM / 11:00 PM |

### Conversion Formula

```
Local Time = UTC + Offset
UTC = Local Time - Offset
```

**Example:**
- You're in New York (UTC-5)
- Current local time is 3:00 PM (15:00)
- UTC = 15:00 - (-5) = 15:00 + 5 = 20:00 UTC

### Online Converters
If you need to convert times:
- [timeanddate.com](https://www.timeanddate.com/worldclock/converter.html)
- [worldtimebuddy.com](https://www.worldtimebuddy.com/)
- Search "current UTC time" in any search engine

## Tips for Using AeroAlarm

### Setting Your First Alarm
1. Determine what UTC time you want the alarm
2. If thinking in local time, convert to UTC first
3. Set the alarm using 24-hour format (00:00 - 23:59)

### Common Scenarios

**Morning Wake-up (New York, EST)**
- Want to wake up at 7:00 AM local
- Convert: 7:00 AM EST = 12:00 UTC
- Set alarm for: 12:00

**Evening Reminder (Tokyo, JST)**
- Want reminder at 8:00 PM local
- Convert: 8:00 PM JST = 11:00 UTC
- Set alarm for: 11:00

**International Meeting**
- Meeting at 3:00 PM UTC
- Just set alarm for: 15:00
- Everyone in the meeting uses the same UTC time

### Verification
Always verify your alarm by comparing:
1. The UTC time shown on the app's clock
2. Your local time
3. The offset between them

Most smartphones display UTC time in Clock app > World Clock by adding a city in the UTC+0 zone (like London or Reykjavik).

## 24-Hour Time Format

Zulu time uses 24-hour format (military time):

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

Great question! While local time works fine for personal use, Zulu time is essential when:

1. **Traveling**: Your alarm stays consistent across time zones
2. **Remote Teams**: No confusion about "9 AM your time or mine?"
3. **Documentation**: Recording events with timestamps that never change
4. **Precision**: Avoiding DST transitions and time zone mistakes

## Additional Resources

- [What is UTC?](https://en.wikipedia.org/wiki/Coordinated_Universal_Time)
- [Time Zone Map](https://www.timeanddate.com/time/map/)
- [UTC Time Now](https://time.is/UTC)
- [Military Time Converter](https://www.militarytime.us/)

## Questions?

Email [support@northernhangar.com](mailto:support@northernhangar.com) or [open a GitHub Issue](https://github.com/nchodge/AeroAlarm_docs/issues/new/choose).
