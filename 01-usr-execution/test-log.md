# Test Execution Log

## Date: 2025-02-05

### Break Phase

Command:
```bash
bash break/path-hijack.sh
ls
```

Result:
[paste actual output showing compromise]

### Detection Phase

Command:
```bash
bash fix/detect-hijack.sh
```

Result:
[paste output showing malicious binary detected]

### Restoration Phase

Command:
```bash
bash fix/restore-trust.sh
ls
```

Result:
[paste output showing trust restored]

## Observations

- Hash table poisoning persisted until explicit flush
- `type` command showed cached path, not filesystem reality
- `strace` was only reliable ground truth
- Immutable flag successfully prevented binary replacement (tested separately)

## Failure Points

- [Document anything that didn't work as expected]
