# SSH keygen Action

The action runs `ssh-kengen` to generate a key pair stored in `private_key.txt` and `public_key.txt`, with `rsa` encryption and 4096 bits by default. You can specify your inputs.

Or just use [the template](https://github.com/gitx-io/ssh-keygen-template) to run a workflow_dispatch action to generate a specified one.

## inputs

```yaml
  comment:
    description: 'A comment to help you to identify the key, e.g. your email etc.'
    required: false
  encryption:
    # dsa | ecdsa | ed25519 | rsa
    description: 'Encryption type'
    required: true
    default: 'rsa'
  bits:
    description: 'Bits'
    required: true
    default: '4096'
```
