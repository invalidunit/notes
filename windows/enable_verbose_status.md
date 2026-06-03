# 更详细的开关机执行任务信息

## 启用更详细的 Windows 开关机执行任务信息

	reg add HKLM\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System /v VerboseStatus /t REG_DWORD /d 1 /f
