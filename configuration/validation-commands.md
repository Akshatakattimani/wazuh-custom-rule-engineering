# Wazuh Rule Validation

## Objective

Validate the custom Wazuh rule before deployment.

## Validation Command

```bash
sudo /var/ossec/bin/wazuh-analysisd -t
```

## Expected Result

The command validates the XML syntax and confirms that the custom rule can be loaded successfully without errors.

## Why Validation Is Important

- Detects XML syntax errors
- Prevents invalid rule deployment
- Confirms the Wazuh manager can parse the custom rule
