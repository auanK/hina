# Hina Protocol Notes

Minimal reverse-engineering notes for the M-VAVE TANK-G communication protocol.

## Device

* Model:
* Firmware:
* VID:
* PID:

## Transport

* USB interface:
* Endpoint IN:
* Endpoint OUT:
* Transfer type:

## Environment

* OS: Windows
* Official software: M-EFCS
* Capture tool: Wireshark + USBPcap

## Captures

| File | Action           | Notes |
| ---- | ---------------- | ----- |
|      | M-EFCS startup   |       |
|      | Change preset    |       |
|      | Change parameter |       |
|      | Save preset      |       |

## Messages

### Unknown

```text
HOST -> TANK-G

??
```

```text
TANK-G -> HOST

??
```

## Findings

No protocol behavior confirmed yet.

## Unknowns

* Initialization / handshake
* Packet structure
* Preset selection
* Parameter IDs
* Parameter values
* Read/write behavior
* Save command
* Checksums

## Notes

Only experimentally confirmed behavior should be documented as part of the protocol.

Firmware update operations are currently out of scope.
