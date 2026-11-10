# Claude Biopython Skill

A skill for using Biopython in computational molecular biology. It guides sequence manipulation, biological file parsing, NCBI database access, BLAST workflows, structural bioinformatics, phylogenetics, and related analyses.

## What It Covers

- **Sequences and file formats:** Work with DNA, RNA, and protein sequences and parse FASTA, GenBank, FASTQ, PDB, and related formats.
- **NCBI access:** Search and retrieve records from PubMed, GenBank, Protein, Gene, and other NCBI databases with Bio.Entrez.
- **BLAST:** Run remote or local searches and parse search results.
- **Alignment:** Perform pairwise and multiple sequence alignment.
- **Protein structures:** Parse PDB and mmCIF files and analyze structure geometry.
- **Phylogenetics:** Read, build, manipulate, and visualize phylogenetic trees.
- **Advanced analysis:** Work with motifs, population genetics, restriction analysis, and sequence statistics.

## Installation

Clone this repository into your Claude skills directory:

```bash
git clone https://github.com/Brajesh31/claude-biopython-skill.git ~/.claude/skills/biopython
```

Install Biopython:

```bash
uv pip install biopython
```

When using NCBI Entrez, configure an email address and optionally an API key:

```python
from Bio import Entrez

Entrez.email = "your.email@example.com"
# Optional: Entrez.api_key = "your_api_key_here"
```

## Using the Skill

Example request:

```text
Use the biopython skill to parse a FASTA file, calculate sequence
statistics, and translate the coding sequences.
```

The skill directs Claude to the appropriate reference for sequence I/O, alignments, databases, BLAST, structures, phylogenetics, or advanced features.

## References

- `references/sequence_io.md`
- `references/alignment.md`
- `references/databases.md`
- `references/blast.md`
- `references/structure.md`
- `references/phylogenetics.md`
- `references/advanced.md`

Use the reference files for detailed APIs and examples. Respect NCBI rate limits, validate input formats, handle network and parsing errors, and document analysis parameters for reproducibility.
