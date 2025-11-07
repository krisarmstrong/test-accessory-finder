# Architecture

## Overview

iPerf Discovery Utility is a Python script designed to locate NetAlly Test Accessories running iPerf3 servers on IPv4 networks. It scans for devices on TCP port 2359 and queries them for identification.

## Core Components

1. **Network Scanner** - Asynchronous network scanning using asyncio
2. **Port Prober** - TCP connection testing on port 2359
3. **Device Query** - Protocol-specific device identification
4. **Logging System** - Detailed debug and result logging

## Technical Implementation

- Uses Python 3 standard library only
- Asynchronous I/O with asyncio for efficiency
- Socket-based TCP communication
- File-based logging and result output
- Configurable timeouts via config file

## Data Flow

```
Network Range → Port Scanner → TCP Probe → Device Query → Result Logging
```

## Design Principles

1. **Efficiency**: Async scanning for speed
2. **Portability**: Standard library only
3. **Reliability**: Comprehensive error handling
4. **Logging**: Detailed debug information

---
Author: Kris Armstrong
