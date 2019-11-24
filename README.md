dnmasscan
=========
dnmasscan is a bash script to automate resolving a file of domain names and subsequentlly scanning them using masscan.

As masscan does not accept domain names, a file is created (specified in the second argument to the script) which will log which IP addresses resolve to which domain names for cross reference after the script has finished executing.

If no masscan options are passed to the script, it will instead use the default options, which are:

```
-p1-65535 -oG masscan.log --rate=500
```

Example Usage
=============
[![asciicast](https://asciinema.org/a/269108.svg)](https://asciinema.org/a/269108)
