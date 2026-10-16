# Hina Protocol Notes

Minimal reverse-engineering notes for the M-VAVE TANK-G communication protocol.

## Device

- Model: M-VAVE TANK-G
- Firmware: Unknown
- VID: 0x4C4A
- PID: 0xC755

## Transport

- USB interface: 4 (MIDI Streaming)
- Endpoint IN: 0x84
- Endpoint OUT: 0x04
- Transfer type: Bulk
- Max packet size: 64 bytes

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

- The device exposes a bidirectional USB-MIDI interface.
- M-EFCS communication protocol is not yet identified.

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
