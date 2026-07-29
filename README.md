# FORE/TRACE

Evidence-bounded lifecycle infrastructure and reviewer artifact for the FORE/TRACE NeurIPS 2026 Creative AI Track paper.

## Canonical reviewer artifact

Download the exact uploaded release asset—not GitHub's automatically generated source archives:

- Release: https://github.com/aarnavt7/FORE-TRACE/releases/tag/v1.1.1
- Artifact: https://github.com/aarnavt7/FORE-TRACE/releases/download/v1.1.1/FORE_TRACE_artifact-v1.1.1.zip
- SHA-256: `94565338953d2eb5908766b53d45e1066dbef28bb9b82fb6bd534476a151d9c6`
- Size: `42,784,856` bytes
- External manifest SHA-256: `b64de1ddf6d999e43d8f4cec65db9d055b52e8bc2f2d7443bbf50aa4f3a6ef25`

Version 1.1.1 is solely a packaging repair that declares and lock-binds Matplotlib 3.11.1. It does not change retained scientific or display bytes, records, protocol, conclusions, privacy boundaries, or analytic-unit accounting. The unpublished v1.1.0 candidate is intentionally not provided.

## Reproduction boundary

The artifact is synthetic-only and contains no participant or private-draft data. Verification is model-free retained-record recomputation, not a new experiment. No model, encoder, or external API calls are required by the documented verification path.

After extracting the canonical ZIP into an empty directory:

```bash
uv sync --locked --all-extras --python 3.13.9
make reproduce-main
make regenerate-assets-v1.1
```

See the packaged `README.md`, `REPRODUCIBILITY.md`, `DATA_CARD.md`, `RESOURCES_AND_ASSETS.md`, checksum ledger, and machine-readable manifest for the complete protocol and evidence boundaries.

## Licensing

Original code and documentation are provided under the MIT License. Author-controlled synthetic fixtures and retained synthetic material are provided under CC BY 4.0 to the extent the author holds the relevant rights. Third-party dependencies and model references remain governed by their upstream terms; model weights are not redistributed.
