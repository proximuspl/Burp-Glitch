# Burp-Glitch
Replace your vmoptions file or add mentioned parameters in your file in order to fix visual glitches that may occur in Burp Suite Pro (tester on 2023.9.4 ver) on Windows 10/Windows 11 with two monitors or 4k hdr monitor.

* BurpSuitePro.vmoptions:
```
# Location file (default Win11): C:\Users\<username>\AppData\Local\Programs\BurpSuitePro\BurpSuitePro.vmoptions 
# Parameters to fix windows glitches (second monitor / 4k hdr) 
# Enter one VM parameter per line
# For example, to adjust the maximum memory usage to 512 MB, uncomment the following line:
# -Xmx512m
# To include another file, uncomment the following line:
# -include-options [path to other .vmoption file]

-XX:MaxRAMPercentage=50
-include-options user.vmoptions
-Dsun.java2d.noddraw=true  
-Dsun.java2d.d3d=false  
-Dswing.useflipBufferStrategy=True  
-Dsun.java2d.ddforcevram=true  
-Dsun.java2d.ddblit=false
```
