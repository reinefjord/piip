# piip
Small bash script for tracking which and how many hours you've worked.

## Installation
Create `~/.piip/` or change the `DB` variable to whatever you want. That's
pretty much it. A good idea is to add the script to `$PATH`.

This script makes use of Bash >=4 features.

The GNU `date` and BSD `date` are not compatable, set the `$DATEBIN` variable
to you GNU `date` if your default `date` is BSD. If you are on OS X for
example, install `coreutils` with `brew` and set `$DATEBIN` to `gdate`.

## Usage
```
piip in             Start tracking time
piip out            Stop tracking time
piip count          Print how many hours you've worked each day
piip edit           Edit the plaintext database with your $EDITOR
piip check_health   Check the health of the database (is run automatically with "count")
```

## Disclaimer
I made this to track my own hours, look through the code to see if it'll work
for you. Tracking time between days will probably not work. Not sure what will
happen and can't be bothered to check :)
