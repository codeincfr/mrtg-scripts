# CPU monitoring script

The CPU usage is read using `mpstat`. This program is part of the `sysstat` package which can be installed running:
`apt-get install sysstat`

## MRTG Configuration
```
#---------CPU-------------------
Target[cpu]: `/etc/mrtg/cpu.php`
Options[cpu]: nopercent,growright,gauge,noinfo,nobanner
#Unscaled[cpu]:dwmy
MaxBytes[cpu]: 100
YLegend[cpu]: % CPU
ShortLegend[cpu]: % CPU
Legend1[cpu]: % CPU User
Legend2[cpu]: % CPU User + Sys
LegendI[cpu]: User:
LegendO[cpu]: Total:
Title[cpu]: CPU
PageTop[cpu]: <h1>CPU</h1>
WithPeak[cpu]:wmy
Legend3[cpu]: Max % CPU User
Legend4[cpu]: Max % CPU USer + Sys
#--------end CPU-----------------------------
```
