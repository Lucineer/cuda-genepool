# cuda-genepool

Gene pool — shared pattern library for agent evolution and code sharing

Part of the Cocapn biology layer — bio-inspired agent lifecycle and energy.

## What It Does

### Key Types

- `Gene` — core data structure
- `Enzyme` — core data structure
- `RnaMessenger` — core data structure
- `DecodedIntent` — core data structure
- `Protein` — core data structure
- `ExecutionResult` — core data structure
- _and 10 more (see source)_

## Quick Start

```bash
# Clone
git clone https://github.com/Lucineer/cuda-genepool.git
cd cuda-genepool

# Build
cargo build

# Run tests
cargo test
```

## Usage

```rust
use cuda_genepool::*;

// See src/lib.rs for full API
// 31 unit tests included
```

### Available Implementations

- `Instinct` — see source for methods
- `Gene` — see source for methods
- `Enzyme` — see source for methods
- `RnaMessenger` — see source for methods
- `Protein` — see source for methods
- `Genome` — see source for methods

## Testing

```bash
cargo test
```

31 unit tests covering core functionality.

## Architecture

This crate is part of the **Cocapn Fleet** — a git-native multi-agent ecosystem.

- **Category**: biology
- **Language**: Rust
- **Dependencies**: See `Cargo.toml`
- **Status**: Active development

## Related Crates

- [cuda-energy](https://github.com/Lucineer/cuda-energy)
- [cuda-neurotransmitter](https://github.com/Lucineer/cuda-neurotransmitter)
- [cuda-biology](https://github.com/Lucineer/cuda-biology)
- [cuda-dna](https://github.com/Lucineer/cuda-dna)

## Fleet Position

```
Casey (Captain)
├── JetsonClaw1 (Lucineer realm — hardware, low-level systems, fleet infrastructure)
├── Oracle1 (SuperInstance — lighthouse, architecture, consensus)
└── Babel (SuperInstance — multilingual scout)
```

## Contributing

This is a fleet vessel component. Fork it, improve it, push a bottle to `message-in-a-bottle/for-jetsonclaw1/`.

## License

MIT

---

*Built by JetsonClaw1 — part of the Cocapn fleet*
*See [cocapn-fleet-readme](https://github.com/Lucineer/cocapn-fleet-readme) for the full fleet roadmap*
