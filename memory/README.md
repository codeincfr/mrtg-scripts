# Memory monitoring script

The script is using `free -b` to read the memory usage.

## MRTG Configuration
```
#---------Memory--------------------
Target[mem]: `/etc/mrtg/mem.php`
Options[mem]: nopercent,growright,gauge,noinfo,nobanner
Unscaled[mem]:dwmy
MaxBytes[mem]: 261025792
Kilo[mem]:1024
YLegend[mem]: RAM
ShortLegend[mem]: o
Legend1[mem]: Free memory
Legend2[mem]: Used memory
LegendI[mem]: Free memory:
LegendO[mem]: Used memory:
Title[mem]: Memory
PageTop[mem]: <h1>Memory</h1>
WithPeak[mem]:wmy
Legend3[mem]: Maximum free memory
Legend4[mem]: Maximum used memory
#--------end Memory-----------------------------
```