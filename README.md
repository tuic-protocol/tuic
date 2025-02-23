# TUIC Protocol

[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
[![GitHub License](https://img.shields.io/github/license/tuic-protocol/tuic)](LICENSE)

TUIC defines a standardized network proxy protocol for relaying TCP and UDP traffic.

## Motivation

- Proxying TCP and UDP traffic in 0-RTT.
- Achieving [Full Cone](https://www.rfc-editor.org/rfc/rfc3489#section-5) NAT compatibility for UDP proxying.
- Supporting both lossy and lossless (via streams) UDP proxying.
- Leveraging the advantages of QUIC, including:
    - Integrated secure transport and reliable data transfer.
    - Bidirectional user-space congestion control.
    - Stream multiplexing.
    - Connection migration.
- Prioritizing simplicity, flexibility, and future extensibility.

There is no official implementation of the TUIC protocol in this repository. This is to focus on the protocol design itself and avoid duplicating efforts on features already well-established in other implementations.

## Specification

TUIC is standardized as an implementation-agnostic protocol. The protocol specification is defined in [SPEC.md](https://github.com/tuic-protocol/tuic/blob/master/SPEC.md).

For a specific protocol version, implementation changes are not expected. However, different protocol versions are not guaranteed to be compatible with each other.

The latest protocol version is `0x05`.

## Implementations

Third-party implementations of the TUIC protocol are a fundamental part of the community and are highly appreciated and encouraged.

The implementations listed below are sorted alphabetically by name. Note that front-end applications based on other implementations are not listed here.

If your implementation is not listed, feel free to open a pull request to add it.

### Server Side

| Name | Open Source |
| - | - |
| [mihomo](https://github.com/MetaCubeX/mihomo) | Yes |
| [sing-box](https://github.com/SagerNet/sing-box) | Yes |
| [tuic (Itsusinn/tuic)](https://github.com/Itsusinn/tuic) | Yes |

### Client Side

| Name | Supported Platforms | Open Source |
| - | - | - |
| [ClashRS](https://github.com/Watfaq/clash-rs) | Cross-platform | Yes |
| [dae](https://github.com/daeuniverse/dae) | Linux | Yes |
| [mihomo](https://github.com/MetaCubeX/mihomo) | Cross-platform | Yes |
| [Shadowrocket](https://shadowlaunch.com/) | iPhone/iPad/Apple TV | No |
| [sing-box](https://github.com/SagerNet/sing-box) | Cross-platform | Yes |
| [Stash](https://stash.ws) | Apple platforms | No |
| [Surge](https://nssurge.com/) | Apple platforms | No |
| [tuic (Itsusinn/tuic)](https://github.com/Itsusinn/tuic) | Cross-platform | Yes |

## Contributing

The TUIC community welcomes and appreciates all contributions. Before contributing, please review our [Code of Conduct](https://github.com/tuic-protocol/tuic/blob/master/CODE_OF_CONDUCT.md) and [Contributing Guidelines](https://github.com/tuic-protocol/tuic/blob/master/CONTRIBUTING.md).

English is the preferred language for communication in this repository.

[Learn more about why the TUIC project is being restarted (posted in Simplified Chinese)](https://www.eaimty.com/2025/restart-developing-tuic-but-not-as-the-author)

## License

This repository is licensed under the [GNU General Public License v3.0](https://github.com/tuic-protocol/tuic#GPL-3.0-1-ov-file).

However, the concept of the TUIC protocol is license-free. The protocol itself is not trademarked or patented. You can implement, modify, and redistribute the protocol without any restrictions.
