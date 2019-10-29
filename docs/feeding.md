---
id: feeding
title: Feeding
---

## What is Feeding?

Feeding is the act of pushing your decoded data up to an aggregator. Aggregating feed data allows others to see your data. Feeding gives you all the feels.
More data helps us develop this out to be more useful. Send your ACARS and VDL2 traffic.

## How to Feed

### ACARS

#### acarsdec

```
acarsdec -v -o 4 -g 40 **-i XX-YYYYZ -j airframes.io:5550** -r 0 131.550 131.525 131.725 131.825 130.025 130.425 130.450 131.125
```

The important stuff is marked in bold.

Your identifier (indicated by the "-i" parameter) can be whatever you want it to be. Our recommendation is to use the XX-YYYYZ format, where XX is a two digit representation of your initials or other personal identifier (mine is KE), YYYY is the nearest airport to you (mine is KMHR) and Z is the receiver number (in case you have multiple in the same locale). You are welcome to add additional identifiers to the end of it (such as -ACARS or -VDL2) to further clarify.

Be sure to use the correct values for gain, output (your local terminal), and the frequencies to scan. They may be very different from the ones I provide in the example above.
