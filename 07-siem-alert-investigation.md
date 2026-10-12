# 07 · How to Investigate a SIEM Alert

> An alert is a **lead**, not proof of compromise.

1. **Understand the alert:** rule, severity, triggering fields, data source, time, entities involved
2. **Validate & scope:** confirm time/timezone; check events before and after, isolated or part of a sequence?
3. **Correlate:** pivot on user, device, IPs, process, domain, URL, hash across auth, email, network, endpoint logs
4. **Investigate by type:** email (sender, links, attachments) · network (connections, DNS/HTTP) · endpoint (process ancestry, file activity, persistence)
5. **Verdict:** benign · false positive · likely true positive · inconclusive/escalate; record timeline, evidence for and against, affected assets, indicators
6. **Respond within process:** escalate or contain only within authorization and playbook; document actions and rationale

## Analyst checks
- Severity or a single indicator is not the verdict
- Look for legitimate explanations (approved admin work, known software, business process)
- Preserve logs, state what's unknown, make the next action clear
