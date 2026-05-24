# Wiki Log

> Chronological record of all wiki actions. Append-only.
> Format: `## [YYYY-MM-DD] action | subject`
> Actions: ingest, update, query, lint, create, archive, delete
> When this file exceeds 500 entries, rotate: rename to log-YYYY.md, start fresh.

## 2026-05-23 create | Wiki initialized
- Domain: exercise (low-impact strength, yoga, stretching, cardiac recovery, over-50 male)
- Structure created with SCHEMA.md, index.md, log.md
- Raw source ingestion: 10 articles added to raw/
## 2026-05-23 ingest | 10 source articles
- raw/AHA_ACC_AACVPR_2024_Core_Components.md
- raw/cardiac-recovery-fitness-protocol-deep-research.md
- raw/Clinical_Review_of_Cardiac_Rehabilitation_Phases.md
- raw/Exercise_Progression_and_GXT_Standards.md
- raw/Low_Impact_and_Functional_Fitness_Over_50.md
- raw/Optimizing_Exercise_Volume_for_Secondary_Prevention.md
- raw/Physiology_and_Risks_of_the_Valsalva_Maneuver.md
- raw/Resistance_Training_Entry_Timelines_and_Precautions.md
- raw/Resistance_Training_Guidelines_and_Hemodynamics.md
- raw/Yoga_for_Heart_Health_Safety_and_Contraindications.md
## 2026-05-23 create | Concepts: Static Stretching + Dynamic Flexibility
- docs/concepts/static-stretching.md
- docs/concepts/dynamic-flexibility.md
## 2026-05-23 lint | SCHEMA.md fixes
- Defined full tag taxonomy (13 tags across domain/clinical/population categories)
- Fixed `contractions` -> `contradictions` typo in Update Policy
## 2026-05-23 update | index.md sync
- Updated page count: 2 -> 14
- Added dynamic-flexibility to Concepts section
- Set last updated date
## 2026-05-23 create | Cardiac Rehabilitation Phases (concept)
- docs/concepts/cardiac-rehabilitation-phases.md
- Sources: 3 source files (Clinical_Review, cardiac-recovery-deep-research, AHA 2024)
- Content: Phase I-IV framework, intake assessment, ITP requirements
## 2026-05-23 create | Valsalva Maneuver (concept)
- docs/concepts/valsalva-maneuver.md
- Sources: 2 source files (Physiology_and_Risks, cardiac-recovery-deep-research)
- Content: 4-phase hemodynamic model, contraindication list, correct breathing protocol
## 2026-05-23 create | Yoga for Cardiac Recovery (concept)
- docs/concepts/yoga-for-cardiac-recovery.md
- Sources: 2 source files (Yoga_Safety, cardiac-recovery-deep-research)
- Content: 5 contraindication categories, 5 safe alternatives, Pranayama warnings
## 2026-05-23 create | Low-Impact Cardio Modalities (concept)
- docs/concepts/low-impact-cardio-modalities.md
- Sources: 2 source files (Low_Impact_Fitness, cardiac-recovery-deep-research)
- Content: 5 modalities (rowing, swimming, walking, cycling, bands), sample weekly schedule
## 2026-05-23 create | Aerobic Exercise Prescription (concept)
- docs/concepts/aerobic-exercise-prescription.md
- Sources: 2 source files (Exercise_Progression_GXT, cardiac-recovery-deep-research)
- Content: Karvonen formula, Borg RPE scale, duration-first progression rule
## 2026-05-23 create | Exercise Volume for Secondary Prevention (concept)
- docs/concepts/exercise-volume-secondary-prevention.md
- Sources: 2 source files (Volume_Secondary_Prevention, AHA 2024)
- Content: 4 volume tiers (1000/1500/2200 kcal/wk), MET-minute formula, mortality correlation
## 2026-05-23 create | Resistance Training Entry Timeline (concept)
- docs/concepts/resistance-training-entry-timeline.md
- Sources: 3 source files (RT_Entry_Timelines, AHA 2024, cardiac-recovery-deep-research)
- Content: MI/PCI/CABG timelines, sternal precautions, pacemaker/ICD precautions
## 2026-05-23 create | Entity: Rowing
- docs/entities/rowing.md
- Sources: Low_Impact_Fitness, cardiac-recovery-deep-research
## 2026-05-23 create | Entity: Recumbent Cycling
- docs/entities/recumbent-cycling.md
- Sources: Low_Impact_Fitness, cardiac-recovery-deep-research
## 2026-05-23 create | Entity: Yoga
- docs/entities/yoga.md
- Sources: Yoga_Safety, cardiac-recovery-deep-research
## 2026-05-23 create | Entity: Tai Chi
- docs/entities/tai-chi.md
- Sources: Clinical_Review, cardiac-recovery-deep-research, Low_Impact_Fitness
## 2026-05-24 fix | All cross-links repaired across 13 files
- Converted concept page links from `concepts/other` → `../other` (was double-nested)
- Converted entity page links from `entities/other` → `../concepts/other` or `../entities/other`
- Removed self-referential link from valsalva-maneuver.md
## 2026-05-24 create | Risk Stratification (concept) + .gitignore
- docs/concepts/risk-stratification.md - AACVPR risk classification algorithm
- .gitignore created (site/, __pycache__, etc.)
## 2026-05-24 create | Comparison: Tai Chi vs Yoga for Cardiac Recovery
- docs/comparisons/tai-chi-vs-yoga.md
- Head-to-head analysis across 12 dimensions with clinical prescription guidance
## 2026-05-24 ingest | Synthesized Resistance Training Guidelines & Hemodynamics
- Added prescription guidelines table and hemodynamic safety section to resistance-training-entry-timeline.md
- Key finding: high-rep sets produce higher BP spikes than heavy-load sets — fatigue management > load management
## 2026-05-24 create | Comparison: Rowing vs Recumbent Cycling
- docs/comparisons/rowing-vs-recumbent-cycling.md
- 12-dimension comparison with Phase-based sequencing strategy
## 2026-05-24 create | Query: Beta-Blockers and Exercise Prescription
- docs/queries/beta-blockers-exercise-prescription.md
- Full clinical guide: HR targets, RPE reliance, modality preferences, safety monitoring
## 2026-05-24 create | Entity: Swimming
- docs/entities/swimming.md
- Water walking (Phase II) through lap swimming (Phase IV); stroke considerations, hydrostatic benefits
