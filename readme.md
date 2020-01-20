# Low battery monitor

A simple battery monitor written in Rust. Called with arguments to specifiy at which battery percentages notifications should be sent:

```
low-battery -l 10 -c 5
```

Where `l` in the first (low) notification and `c` is the second (critical). 

Scans every 2 minutes unless battery is above 30% where the interval is increased to 10 minutes.