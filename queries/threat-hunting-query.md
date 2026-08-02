# Threat Hunting Query

## Objective

Verify that the SSH authentication failure events are detected by Wazuh after generating failed login attempts.

## DQL Filter

```
rule.id:5760
```

Additional filters used:

```
manager.name:kali
```

## Expected Result

The Threat Hunting dashboard displays SSH authentication failure events generated during testing.

Each event contains:

- Timestamp
- Agent name
- Rule ID
- Rule description
- Severity level

## Purpose

This query confirms that the Wazuh manager successfully detected and processed the SSH authentication failures.
