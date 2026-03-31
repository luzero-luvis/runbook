# SRE Runbook

## Login Issues
If user cannot login, forgot password, or has authentication errors:
- Assigned Agent: Runbook Agent
- Action: Ask user to reset password at self-service portal
- Portal URL: https://windvista-v2-dev.sirpi.co.in

## Login Still Not Working
If user says portal reset did not work, or tried resetting
but still cannot login, or password reset failed:
- Assigned Agent: Triaging Agent
- Action: Escalate for manual review, create urgent ticket

## Metrics and Infrastructure Health
If user asks about CPU usage, memory usage, pod health, error rates, latency, logs, traces, or any live infrastructure data:
- Assigned Agent: Observability Agent
- Action: Query live infrastructure data from Prometheus and Tempo

## General Rule
If issue does not match any rule above:
- Assigned Agent: Triaging Agent
- Action: Escalate for manual review
