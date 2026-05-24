# Exercise Wiki

A living knowledge base for low-impact fitness, cardiac rehabilitation, and heart-healthy exercise programming — with a focus on recovery after cardiovascular events and sustainable strength for the over-50 male.

## Domain

Low-impact strength training for foundational health; integrating yoga, specialized stretching & flexibility routines, cardio recovery specifically after cardiovascular events (e.g., heart attack), and designing fitness programming tailored to middle-aged adults. This wiki synthesizes clinical guidelines (AHA/ACC/AACVPR, ACSM), peer-reviewed research, and practical rehabilitation protocols.

## Quick Start

### Local Development

```bash
# Install MkDocs with Material theme
pip install mkdocs-material

# Serve locally with live reload
mkdocs serve

# Build static site
mkdocs build
```

### Viewing the Published Site

The wiki is deployed to GitHub Pages on every push to `main`. Visit:

[https://humanshell.github.io/exercise-wiki/](https://humanshell.github.io/exercise-wiki/)

## Structure

```
docs/
├── index.md                 # Content catalog
├── log.md                   # Chronological history of all actions
├── concepts/                # Explanatory pages (CR phases, aerobic Rx, Valsalva, etc.)
├── entities/                # Modality pages (rowing, cycling, yoga, tai chi, swimming)
├── comparisons/             # Side-by-side analyses
└── queries/                 # Answers to difficult questions
raw/                         # Source articles from clinical guidelines and journals
mkdocs.yml                   # MkDocs configuration
SCHEMA.md                    # Wiki schema, conventions, tag taxonomy, and update policy
```

## Content Conventions

All pages use YAML frontmatter with `title`, `created`/`updated` dates, `type` (concept/entity/comparison/query), controlled-vocabulary `tags`, and `sources`. Every claim sourced from a raw article is marked with provenance markers (`^[raw/file.md]`). See `SCHEMA.md` for full conventions.

## Pages (19 total)

**Concepts (10):** Cardiac Rehabilitation Phases, Aerobic Exercise Prescription, Exercise Volume for Secondary Prevention, Low-Impact Cardio Modalities, Resistance Training Entry Timeline, Valsalva Maneuver, Yoga for Cardiac Recovery, Static Stretching, Dynamic Flexibility, Risk Stratification

**Entities (5):** Rowing, Recumbent Cycling, Yoga, Tai Chi, Swimming

**Comparisons (2):** Tai Chi vs Yoga, Rowing vs Recumbent Cycling

**Queries (1):** Beta-Blockers and Exercise Prescription
