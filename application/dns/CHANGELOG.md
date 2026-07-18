# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.1.0](https://github.com/RawSocketLabs/protocols/compare/dns-v0.0.3-pre1...dns-v0.1.0) - 2026-07-04

### Added

- *(dns)* add DNS-over-TCP fallback to the resolver ([#14](https://github.com/RawSocketLabs/protocols/pull/14))
- *(dns)* add a synchronous UDP resolver client (client feature) ([#11](https://github.com/RawSocketLabs/protocols/pull/11))
- *(dns)* [**breaking**] adopt WireLen for auto-deriving counts and rdlength ([#6](https://github.com/RawSocketLabs/protocols/pull/6))
- *(dns)* add encode-side name compression (to_compressed_bytes) ([#4](https://github.com/RawSocketLabs/protocols/pull/4))

### Fixed

- *(dns)* enforce the 255-byte name limit and reject empty labels ([#8](https://github.com/RawSocketLabs/protocols/pull/8))
- *(dns)* prevent SRV/CAA count underflow panic and keep compressed rdlength honest ([#7](https://github.com/RawSocketLabs/protocols/pull/7))

### Other

- *(dns)* source blessed externals via rsl-deps (rand); keep thiserror direct
- *(dns)* use the renamed #[bw(auto_len = …)] WireLen directive ([#20](https://github.com/RawSocketLabs/protocols/pull/20))
- *(dns)* add SRV/CAA/OPT refcheck annotations and refresh the crate doc ([#10](https://github.com/RawSocketLabs/protocols/pull/10))
- *(dns)* layer the tests (unit/component/integration) + add examples ([#3](https://github.com/RawSocketLabs/protocols/pull/3))
