# Wiki Schema

## Domain
Low impact strength training for foundational health; integrating yoga, specialized stretching & flexibility routines, cardio recovery specifically after cardiovascular events (e.g., heart attack), and designing fitness programming tailored to the needs of a 50-year-old male. This wiki is focused on safe, sustainable, long-term improvements in strength and resilience.

## Conventions
- File names: lowercase, hyphens, no spaces (e.g., `cardio-progression.md`)
- Every wiki page starts with YAML frontmatter (see below)
- Use `[[wikilinks]]` to link between pages (minimum 2 outbound links per page for all entity/concept pages)
- When updating a page, always bump the `updated` date
- Every new page must be added to `index.md` under the correct section
- Every action must be appended to `log.md`
- **Provenance markers:** On pages that synthesize 3+ sources, append `^[raw/articles/source-file.md]` at the end of paragraphs whose claims come from a specific source. This lets a reader trace each claim back without re-reading the whole raw file. Optional on single-source pages where the `sources:` frontmatter is enough.

## Frontmatter
  ```yaml
  ---
  title: Page Title
  created: YYYY-MM-DD
  updated: YYYY-MM-DD
  type: entity | concept | comparison | query | summary
  tags: [from taxonomy below]
  sources: [raw/articles/source-name.md] # Only required for sourced content
  # Optional quality signals:
  confidence: high | medium | low        # how well-supported the claims are
  contested: true                        # set when the page has unresolved contradictions, e.g., a debate exists in the community
  contradictions: [other-page-slug]      # pages this one conflicts with
  ---
  ```

# Note on Frontmatter: The `title`, `type`, and `tags` are mandatory. Confidence and Contradictions fields improve content quality control.

## Tag Taxonomy
\[Define 10-20 top-level tags for the exercise domain here. Suggested high-level tags include: `muscle-group`, `exercise-type`, `training-style`, `physiology`, `injury-risk`, `equipment`.]

Rule: every tag on a page must appear in this taxonomy. If a new tag is needed, add it to this section first, then use it. This prevents tag sprawl.

## Page Thresholds
- **Create a page** when an entity/concept appears in 2+ sources OR is central to one source.
- **Add to existing page** when a source mentions something already covered.
- **DON'T create a page** for passing mentions, minor details, or things outside the domain.
- **Split a page** when it exceeds ~200 lines — break into sub-topics with cross-links.
- **Archive a page** when its content is fully superseded — move to `_archive/`, remove from index and update all linking pages.

## Entity Pages (e.g., Human, Bench Press)
One page per notable entity. Include:
- Overview / what it is
- Key facts and dates
- Relationships to other entities (`[[wikilinks]]`)
- Source references

## Concept Pages (e.g., Progressive Overload)
One page per concept or topic. Include:
- Definition / explanation
- Current state of knowledge
- Open questions or debates
- Related concepts (`[[wikilinks]]`)

## Comparison Pages (e.g., Squat vs Deadlift)
Side-by-side analyses. Include:
- What is being compared and why
- Dimensions of comparison (table format preferred)
- Verdict or synthesis
- Sources

## Update Policy
When new information conflicts with existing content:
1. Check the dates — newer sources generally supersede older ones.
2. If genuinely contradictory, note both positions with dates, links, and sources.
3. Mark the contradiction in frontmatter: `contractions: [page-name]`.
4. Flag for user review by setting `contested: true` or `confidence: low`.