## Log Analysis – SSH Authentication Failure

### Event Observed
Multiple failed SSH login attempts detected from a single IP.

### Key Indicators
- Repeated login failures
- Target account: root
- Same source IP

### Analysis
This pattern indicates a brute-force attempt where an attacker tries multiple passwords.

### Risk
If successful, attacker could gain unauthorized access.

### Mitigation
- Disable root login
- Enable account lockout
- Monitor repeated login attempts
