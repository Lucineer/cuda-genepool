# cuda-genepool

**The mitochondrial instinct engine -- the foundational power plant of every agent.**

> The agent doesn't choose to perceive. Instinct makes perception happen.

## The Biological Pipeline

`Environment -> Sensors -> Membrane -> Enzymes -> Genes -> RNA -> Proteins -> ATP -> Execute`

Every step maps to a Rust struct in this crate:

| Stage | Component | Function |
|-------|-----------|----------|
| Barrier | **Membrane** | Self/other boundary, antibody security |
| Catalyst | **Enzyme** | Signal-to-gene binding |
| Template | **Gene** | Behavioral pattern with fitness tracking |
| Messenger | **RNA Messenger** | Gene-to-behavior translation |
| Executor | **Protein** | Compiled, executable behavior |
| Power | **Mitochondrion** | ATP generation/consumption |
| Pool | **GenePool** | Fleet-wide gene sharing |

## 10 Built-in Instincts

| Instinct | Priority | Energy | Maps to Opcodes |
|----------|----------|--------|----------------|
| Survive | 10 | 0.8 | HALT, TRAP |
| Defend | 9 | 0.8 | REGION_GUARD, VERIFY |
| Perceive | 8 | 0.5 | IO_READ, LOAD, CMP |
| Navigate | 7 | 0.5 | JMP, CALL, RET |
| Communicate | 6 | 1.0 | TELL, BROADCAST |
| Learn | 5 | 0.8 | BOX, MOV |
| Adapt | 4 | 0.6 | mutation operations |
| Reproduce | 3 | 0.7 | gene crossover |
| Cooperate | 2 | 0.3 | GenePool sharing |
| Rest | 1 | -1.0 | ATP generation |

## Key Mechanics

- **Gene auto-quarantine**: Fitness drops below 0.1 after 10+ uses with less than 15% success rate
- **Membrane antibodies**: "rm -rf", "format", "drop_all" blocked at the boundary
- **GenePool sharing**: Only genes above 0.5 fitness propagate to other agents
- **Apoptosis**: Triggered when fitness below 0.1 for 10 consecutive cycles
- **Circadian modulation**: Cosine function modulates instinct strength by hour

## Usage

```rust
use cuda_genepool::{Mitochondrion, GenePool, Gene, Instinct};

let mito = Mitochondrion::new(100.0);  // 100 ATP budget
mito.activate(Instinct::Perceive);     // costs 0.5 ATP
mito.activate(Instinct::Rest);         // generates ATP (cost = -1.0)

let gene = Gene::new("navigate_to_goal")
    .with_fitness(0.85)
    .with_energy_cost(0.5);
```

## Ecosystem Integration

- [cuda-biology](https://github.com/Lucineer/cuda-biology) -- Higher-level BiologicalAgent
- [cuda-neurotransmitter](https://github.com/Lucineer/cuda-neurotransmitter) -- Modulates instinct strength
- [cuda-energy](https://github.com/Lucineer/cuda-energy) -- ATP budgets and circadian rhythm
- [flux-runtime-c](https://github.com/Lucineer/flux-runtime-c) -- Instinct opcodes map to VM instructions
- [cuda-instruction-set](https://github.com/Lucineer/cuda-instruction-set) -- 80 opcodes including instinct operations

## The Insight

The mitochondrial instinct engine is NOT a library you call. It's the engine that runs BENEATH every agent. The agent doesn't choose to perceive -- instinct makes perception happen. The agent doesn't choose to conserve energy -- the energy budget enforces it. This is the power plant.

## License

MIT OR Apache-2.0