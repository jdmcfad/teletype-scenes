### Keys

`alt-Esc` to enter scene save mode.

`alt-Fn` to edit corresponding script.

### Metronome

```
M
M i
M.ACT b
```

Get metronome interval.  Set metronome interval to `i`ms.  Set metronome state to boolean `b`.

### Binary scale degrees

```
N.B d
N.B r s
```

`r` is the starting semitone. E.g., C is `0`.  `s` is the selected semitones specified as a bit pattern.  Use the `R` sigil to specify bits in low-to-high left-to-right order.  For example, C major is `R101011010101`.

### Pattern looping

Set a pattern `p` to its working end (such that `PN.NEXT` would return the beginning value):

```
PN.I p PN.START p
```

Increment then get:

```
PN.NEXT p
```

### Hardware

```
V x
```

Convert `x` to volts.

```
CV n v
```

Set CV `n` to value `v`.

```
PRM
```

Get the value of the PARAM knob.
