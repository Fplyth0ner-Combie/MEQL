# APPLY
Investigate potential attack indicators in the enterprise environment

# Attack-Indicator/miHoYo-Driver-Abuse.meql
Look for potential abuse of the miHoYo mhyprot2.sys driver, \
which is supposed to be used as an anti-cheat feature in the miHoYo's game, \
but it has been proven that it can be exploited for potentially malicious behavior. \
If you find relevant search results, take them seriously. \
If you have determined that your environment should not have it, thoroughly investigate the events. \
Reference: \
https://www.virustotal.com/gui/file/509628b6d16d2428031311d7bd2add8d5f5160e9ecc0cd909f1e82bbbb3234d6/details \
https://www.trendmicro.com/en_us/research/22/h/ransomware-actor-abuses-genshin-impact-anti-cheat-driver-to-kill-antivirus.html

# Attack-Indicator/ProcExp-Driver-Abuse.meql
Look for potential abuse of the Sysinternals procexp152.sys driver, \
It is a driver for the legitimate system analysis tool Process Explorer, \
however, it has no constraints on the caller, \
leading some malicious actors to abuse it for destructive activities such as evading or killing endpoint protection processes. \
Please carefully audit all the results of this query and find evidence that they legitimately exist. \
Otherwise, these results may indicate a highly dangerous cyber attack in progress. \
Reference: \
https://labs.jumpsec.com/a-defenders-guide-for-rootkit-detection-episode-1-kernel-drivers/ \
https://forum.eset.com/topic/31580-process-explorer-detected/ \
https://www.rapid7.com/blog/post/2021/12/13/driver-based-attacks-past-and-present/
