# Ubaidu Architecture
*Technical overview for contributors*

---

## Overview

Ubaidu uses a three-layer architecture designed for maximum pattern discovery with minimal computational overhead. Each layer operates independently, communicating through defined interfaces.

---

## Layer 1: The Gatherer (Thread Collection)

**Purpose:** Acquire and normalize data from diverse sources.

**Components:**

- `source_handlers/` - Modular connectors for different data types:
  - `text_handler.py` - Oral traditions, academic papers, mythological texts
  - `geo_handler.py` - Geological survey data, satellite imagery, terrain maps
  - `patent_handler.py` - Historical patent databases, technology records
  - `linguistic_handler.py` - Language drift patterns, etymological data
  - `genetic_handler.py` - Public genomic databases, population studies

- `normalizers/` - Convert diverse formats to unified thread structure
- `thread_store/` - Lightweight database of raw threads with metadata

**Philosophy:** The gatherer is indiscriminate. It collects everything. Judgment happens later, if at all.

---

## Layer 2: The Loom (Resonance Detection)

**Purpose:** Identify resonant relationships between threads.

**Components:**

- `resonance_engines/` - Multiple methods for detecting connections:
  - `semantic_engine.py` - Linguistic and conceptual similarity
  - `temporal_engine.py` - Chronological alignment patterns
  - `geospatial_engine.py` - Geographic clustering
  - `symbolic_engine.py` - Cross-cultural symbol matching
  - `anomaly_engine.py` - Points where threads *don't* fit expected patterns

- `web_builder.py` - Constructs graph of resonant threads
- `strength_metrics.py` - Quantifies resonance without over-interpreting

**Philosophy:** The loom doesn't claim causation. It only notes that certain threads *vibrate together*. The meaning of that vibration is for later layers.

---

## Layer 3: The Weaver (Human Interface)

**Purpose:** Present resonant patterns for human interpretation.

**Components:**

- `visualization_engine/` - Multiple ways to see the web:
  - `graph_view.py` - Network diagrams of thread connections
  - `timeline_view.py` - Temporal clustering
  - `map_view.py` - Geospatial distribution
  - `narrative_view.py` - Tentative story generation from strong patterns

- `annotation_tools/` - Allow human weavers to add insights back to the web
- `resonance_feedback.py` - Learn from which patterns humans find meaningful

**Philosophy:** The machine finds patterns. Humans find *meaning*. The loop between them is where understanding grows.

---

## Self-Modification Protocol

Ubaidu is designed to improve itself over time. This happens through:

1. **Pattern feedback** - Resonance that leads to verified discoveries strengthens the algorithms that found them
2. **Human guidance** - Weavers can mark which threads and connections feel significant
3. **Cross-layer optimization** - The gatherer learns what kinds of threads tend to produce meaningful resonances

This is not AGI. This is *adaptive heuristics*—a web that learns which threads matter without ever claiming to know *why*.

---

## Current Status

- [ ] Gatherer: Basic text handler implemented
- [ ] Loom: Resonance engine in development
- [ ] Weaver: Visualization layer designed, not built
- [ ] Self-modification: Theoretical framework only

Contributors needed for all layers. See CONTRIBUTING.md for guidelines.
