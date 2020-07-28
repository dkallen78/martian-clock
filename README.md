# Martian Clock

## Wait, What?

It's possible to calculate the time on Mars using the JavaScript Date object, but there's some ugly math involved.

Time on Mars is reckoned in Coordinated Mars Time (MTC). Time on our computer is reckoned in Unix Time (milliseconds since 00:00 Jan 1, 1970). By converting the Unix Time of the JavaScript Date object a few times, we can get to MTC, and from there, determine the hour (1/24th), minute (1/1440th), second (1/86,400th), and millisecond (1/86,400,000th) of the day.

### Unix Time to Julian Date<sub>UTC</sub>

