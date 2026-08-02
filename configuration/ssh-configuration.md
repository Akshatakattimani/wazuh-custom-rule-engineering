# SSH Service Configuration

## Objective

Configure the SSH service to allow password-based authentication for testing the custom Wazuh rule.

## Verify Password Authentication

```bash
sudo sshd -T | grep passwordauthentication
```

Expected Output

```
passwordauthentication yes
```

## Verify SSH Service Status

```bash
sudo systemctl status ssh
```

Expected Result

The SSH service should be active (running), allowing incoming SSH connections from the Windows virtual machine.

## Purpose

- Enable password authentication
- Ensure the SSH service is running
- Prepare the Linux server for authentication testing
