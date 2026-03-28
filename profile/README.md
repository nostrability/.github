# nostrability

Tracking interoperability across the nostr ecosystem.

**[nostrability.github.io/nostrability](https://nostrability.github.io/nostrability/)** — NIP support tracker with per-app compatibility tables

## What is nostrability

- **Positive interop** stuff that works together (e.g. across mutually adopted NIP/kind)
- **Negative interop** where apps break when talking to each other (DMs, zaps, relay lists, etc.)
- **Schema & schema validators** validating nostr events against NIP/kind definitions using JSON Schema
- **Schemata codegen** similar to above but without need for json validators
- **Sherlock** Deducing which  apps post broken stuff to relays
- **Releases** automated daily scanning of nostr repos for new releases

## Key Repos

| Repo | Description |
|------|-------------|
| [nostrability](https://github.com/nostrability/nostrability) | Interoperability tracker. Includes NIP adoption tables, broken interop reports etc. |
| [nostrability web dashboard](https://nostrability.github.io/nostrability/) | the above, rendered |
| [schemata](https://github.com/nostrability/schemata) | Language-agnostic JSON schemas for nostr event validation |
| [sherlock](https://github.com/nostrability/sherlock) |deducing which apps post broken stuff|
| [schemata-codegen](https://github.com/nostrability/schemata-codegen)| typed language constructs that enable the compiler to catch structural mistakes like wrong position, missing field, bad marker value|

### Schemata — language packages

Data packages embed the schemas; validator packages provide `validate()` helpers.

| Language | Data | Validator |
|----------|------|-----------|
| Rust | [schemata-rs](https://github.com/nostrability/schemata-rs) | [schemata-validator-rs](https://github.com/nostrability/schemata-validator-rs) |
| Kotlin | [schemata-kt](https://github.com/nostrability/schemata-kt) | [schemata-validator-kt](https://github.com/nostrability/schemata-validator-kt) |
| Swift | [schemata-swift](https://github.com/nostrability/schemata-swift) | [schemata-validator-swift](https://github.com/nostrability/schemata-validator-swift) |
| Go | [schemata-go](https://github.com/nostrability/schemata-go) | [schemata-validator-go](https://github.com/nostrability/schemata-validator-go) |
| Dart | [schemata-dart](https://github.com/nostrability/schemata-dart) | [schemata-validator-dart](https://github.com/nostrability/schemata-validator-dart) |
| Python | [schemata-py](https://github.com/nostrability/schemata-py) | [schemata-validator-py](https://github.com/nostrability/schemata-validator-py) |
| Java | [schemata-java](https://github.com/nostrability/schemata-java) | [schemata-validator-java](https://github.com/nostrability/schemata-validator-java) |
| PHP | [schemata-php](https://github.com/nostrability/schemata-php) | [schemata-validator-php](https://github.com/nostrability/schemata-validator-php) |
| Ruby | [schemata-ruby](https://github.com/nostrability/schemata-ruby) | [schemata-validator-ruby](https://github.com/nostrability/schemata-validator-ruby) |
| C | [schemata-c](https://github.com/nostrability/schemata-c) | [schemata-validator-c](https://github.com/nostrability/jsonc-daccord) |
| C# | [schemata-csharp](https://github.com/nostrability/schemata-csharp) | [schemata-validator-csharp](https://github.com/nostrability/schemata-validator-csharp) |
| C++ | [schemata-cpp](https://github.com/nostrability/schemata-cpp) | [schemata-validator-cpp](https://github.com/nostrability/schemata-validator-cpp) |

## Resources

- [NIPs](https://github.com/nostr-protocol/nips/) — Nostr Implementation Possibilities (protocol specs)
- [NostrHub](https://nostrhub.io/) — Community NIP extensions and proposals
- [Blossom](https://github.com/hzrd149/blossom) — Blobs stored simply on mediaservers
- [Marmot](https://github.com/marmot-protocol/marmot) — Marmot protocol
- [nostrapps.com](https://nostrapps.com) — Directory of nostr applications
