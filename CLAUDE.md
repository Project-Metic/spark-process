# CLAUDE.md — spark-process

SPARK Process: reST documentation source for the NVIDIA SPARK Process — a reference
process for development and certification of safety-critical software using SPARK 2014 /
Ada. Jointly developed by NVIDIA and AdaCore, reviewed by TÜV-SÜD.

Pre-built: https://nvidia.github.io/spark-process/

Used by Project-Metic as a reference process document for DO-178C-grade compilation
certification and SPARK-verified binary analysis workflows.

## What This Repo Is

A documentation-only repo — reStructuredText sources for the SPARK Process document.
No runtime code. No services. No deployments.

## Key Invariants

- **This is reference documentation, not Metic source code.** Do not add service code here.
- **The process document is a reference, not a Metic requirement.** It informs how Metic
  approaches DO-178C-grade certification but does not replace Metic's own ADRs and specs.
- **Attribution is required.** The document was jointly developed by NVIDIA/AdaCore/TÜV-SÜD.
  Any modifications must preserve attribution headers.

## Dev Commands

```bash
# Build the HTML documentation
make html

# Check links
make linkcheck

# Clean build artifacts
make clean
```

## Tech Stack

- reStructuredText, Sphinx

## Integration with Project-Metic

- Referenced by the `research/` agenda for DO-178C certification approach
- SPARK Process concepts inform proof obligation design for Ada binary lifting targets

## What NOT to Do

- Do not add service code to this documentation repo
- Do not remove attribution headers from the document sources
