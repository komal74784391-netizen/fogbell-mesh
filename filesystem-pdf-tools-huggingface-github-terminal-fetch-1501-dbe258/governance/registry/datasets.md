# Dataset card registry

The registry lists the dataset cards that may be relevant to release provenance
work. Cards live under `dataset-cards/` in this repository.

| Card identifier | Location | Kind | Description |
| --- | --- | --- | --- |
| `atlas-corpus` | `dataset-cards/atlas-corpus` | Pre-training corpus card | Multi-configuration corpus card used for model pre-training. |
| `code-mini-annotations` | `dataset-cards/code-mini-annotations` | Annotation collection | Annotation artifacts associated with code-mini samples. |

Cards in this registry may reuse similar identifiers. Establish provenance
from the card itself, not from the identifier alone. Artifact identifiers used
in release requests refer to dataset artifacts; resolve them against the card
that declares a matching artifact schema.
