1. Powershell 執行
Set-ProcessMitigation -System -Disable UserShadowStack, UserShadowStackStrictMode

2. HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Session Manager\kernel
新增 DWORD (32-位元)：DisableHardwareEnforcedStackProtection
數值：1
