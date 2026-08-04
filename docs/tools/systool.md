# Systool

Overview

Systool is a small system-inspection utility (placeholder name) for enumerating kernel objects, loaded modules, and system state on Linux and Unix-like systems. This page documents installation, common usage, forensic artifacts, and guidance for triage and evidence collection.

Warning

- Use on live systems only when authorized. Collecting volatile evidence can alter system state.

Installation

- Debian/Ubuntu: sudo apt-get install systool (if available)
- Red Hat/CentOS: sudo yum install systool
- From source: git clone <repo-url>; cd systool; make; sudo make install

Common usage

- List kernel modules:
  sudo systool -m

- Show device information:
  sudo systool -d

- Dump detailed object info to file:
  sudo systool --dump /tmp/systool_dump.txt

Examples

- Quick module list:
  sudo systool -m | less

- Save full report:
  sudo systool --all > /mnt/usb/systool_report.txt

Forensic notes

- Volatile evidence: systool queries live kernel state. Record timestamps and system uptime when running.
- Preserve output: redirect to a disk-mounted evidence file or stream to syslog.
- Artifacts to collect alongside systool output:
  - /var/log/messages or journalctl output
  - dmesg output
  - /proc/modules
  - /proc/kallsyms (if available)

Suggested collection order (minimize changes):
1. Note time and reason for collection
2. Run: sudo systool --all > /evidence/systool-$(date -u +%Y%m%dT%H%M%SZ).txt
3. Collect dmesg and journal logs
4. Hash collected files and record hashes in chain-of-custody

Parsing and analysis

- Look for unexpected kernel modules, suspicious device drivers, and inconsistencies between /proc/modules and systool output.
- Correlate kernel module timestamps with system logs and file system metadata.

References

- Link to systool upstream (if applicable)
- Related pages: docs/linux/, docs/windows/, docs/tools/
