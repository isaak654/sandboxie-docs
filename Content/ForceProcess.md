# Force Process

_ForceProcess_ is a sandbox setting in [Sandboxie Ini](SandboxieIni.md). It specifies names of programs. If any of these progams are started outside any sandbox, they will automatically sandboxed in a particular sandbox. For example:

```
   .
   .
   .
   [DefaultBox]
   ForceProcess=iexplore.exe
   ForceProcess=firefox.exe
   [MailBox]
   ForceProcess=outlook.exe
```

The example specifies that Internet Explorer (iexplore.exe) and Firefox (firefox.exe) will be forced to run sandboxed in the sandbox _DefaultBox_. Outlook.exe will be forced to run sandboxed in the sandbox _MailBox_.

Note that the _ForceProcess_ settings only apply to programs that start unsandboxed. If a program is specifically started in a sandbox, or started by a program that is already sandboxed, then _ForceProcess_ settings are not applied.

See also: [ForceFolder](ForceFolder.md). If both a _ForceFolder_ and a _ForceProcess_ are applicable to a program that is starting, the ForceFolder setting takes precedence.

Related [Sandboxie Control](SandboxieControl.md) setting: [Sandbox Settings > Program Start > Forced Programs](ProgramStartSettings.md#forced-programs)

See also: [Program Settings](ProgramSettings.md#page-1).
