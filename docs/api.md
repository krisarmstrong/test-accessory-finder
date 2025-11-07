# API Documentation

## Usage

```bash
python iperf_discovery.py <network_address> [--verbose] [--timeout <seconds>]
```

**Arguments**:
- `network_address`: IPv4 network (e.g., 192.168.1.0/24)
- `--verbose`: Enable verbose console output
- `--timeout`: Socket timeout in seconds (default: 2.0)

**Examples**:
```bash
# Basic scan
python iperf_discovery.py 192.168.1.0/24

# Verbose mode
python iperf_discovery.py 192.168.1.0/24 --verbose

# Custom timeout
python iperf_discovery.py 10.0.0.0/24 --timeout 5
```

## Configuration

Optional config file: `/mnt/mmc3/iperfaccessory.conf`
```ini
[discovery]
timeout = 2.0
```

## Output Files

- `iperfdiscovery.log`: Debug logging
- `iperfaccessory`: Discovered devices

## Dependencies

- Python 3.6+ (standard library only)
- Network access to target subnet
- Write permissions for output files

---
Author: Kris Armstrong
