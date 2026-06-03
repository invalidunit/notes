# 将硬件时钟视为 UTC 时间

让 Windows 将硬件时钟视为 UTC 时间，可以解决 Linux 或者黑苹果之类与 win 切换时时间差不多相差 8 小时的问题

	reg add HKLM\SYSTEM\CurrentControlSet\Control\TimeZoneInformation /v RealTimeIsUniversal /t REG_DWORD /d 1 /f
