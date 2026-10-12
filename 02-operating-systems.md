# 02 · Operating-System Fundamentals

## Windows
- **Filesystem:** NTFS. Know normal locations: `C:\Windows`, `C:\Users`, `C:\Program Files`, `C:\ProgramData`, `C:\Windows\System32`
- **CLI tools:** `ipconfig`, `ping`, `netstat`, `tasklist`, `whoami`, `cd`, `dir`
- **Users/groups/permissions:** standard, admin, local, domain. Permissions: Read, Write, Execute, Modify, Full Control. Misconfigurations enable privilege escalation.
- **Processes:** what is running, who started it, what launched it, what children it spawned, is it expected?
- **Services:** background functionality; abused for persistence/execution
- **Task Scheduler:** abused for persistence
- **Registry:** system/app configuration, startup behavior
- **Windows Firewall:** unexpected rules deserve a look
- **Event Logs:** logons, processes, services, security events, key evidence
- **WMI:** legitimate admin tool; abused for remote execution, recon, persistence

**Investigation chain:** User → Process → File → Service → Registry → Event Log → Network

## Linux
| Path | Purpose |
|------|---------|
| `/` | root |
| `/home` | user directories |
| `/etc` | configuration |
| `/var` | variable data, logs |
| `/tmp` | temporary files |
| `/usr`, `/bin`, `/sbin` | programs and utilities |

**Commands**
- Files: `pwd`, `ls`, `cd`, `cat`, `less`, `cp`, `mv`, `rm`, `mkdir`
- Search: `grep`, `find`
- Users: `whoami`, `id`, `who`, `w`, `groups`
- Processes: `ps`, `top`, `htop`, `kill`
- Network: `ip`, `ss`, `ping`

```bash
ls -la
cd /var/log
grep "failed" auth.log
```

**Permissions:** r/w/x for owner, group, others (e.g. `rwxr-xr--`).
**Investigate:** unexpected processes, odd parent/child relationships, processes running as root, unknown binaries, listening ports, auto-start services, cron jobs and startup scripts.

**Investigation chain:** User → Command → Process → File → Permission → Service → Network → Logs
