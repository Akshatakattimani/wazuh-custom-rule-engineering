# Rule Validation

After creating the custom detection rule, the Wazuh rule configuration was validated before deployment.

## Validation Command

```bash
sudo /var/ossec/bin/wazuh-analysisd -t
```

## Purpose

- Validate XML syntax
- Check for rule configuration errors
- Ensure Wazuh can successfully load the custom rule
