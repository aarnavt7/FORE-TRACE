# FORE/TRACE

Evidence-bounded lifecycle infrastructure and reviewer artifact for the FORE/TRACE NeurIPS 2026 Creative AI Track paper.

## Paper

- Final paper: https://github.com/aarnavt7/FORE-TRACE/releases/download/v1.1.1/FORE_TRACE_NeurIPS_2026_FINAL_PAPER.pdf
- Paper SHA-256: `607e37ddf0d9837aad6b5fef00b153f620e18e9802718708f5a89bc52edcb77a`
- Format: 16 US-letter pages — six main-content pages, two reference pages, and the completed eight-page NeurIPS checklist

The paper reports a synthetic systems study with no participants or private-draft data. One of six SmolLM-128 analytic units passed Gate A locally; neither cross-block rule authorized an aggregate order. The retained-record verification is not an independent replication or a fresh stochastic-generation run.

## Paper authorship

The FORE/TRACE manuscript is authored by Srujan Chilakapati, Aarnav Trivedi, Safwaan Majid, Arnav Mahajan, Pratyay Jakkula, and Saketh Nandam. All six authors contributed equally and share first authorship.

Affiliations:

- **Academies of Loudoun, Leesburg, Virginia:** Srujan Chilakapati and Aarnav Trivedi
- **Rock Ridge High School, Ashburn, Virginia:** Safwaan Majid, Arnav Mahajan, and Saketh Nandam
- **Thomas Jefferson High School for Science and Technology, Alexandria, Virginia:** Pratyay Jakkula

The immutable v1.1.1 reviewer-artifact ZIP predates this paper-title-page update. Its bytes and published digest remain unchanged; current paper authorship is defined by the final paper and this repository/release description.

## Canonical reviewer artifact

Download the exact uploaded release asset, not GitHub's automatically generated source archives:

- Release: https://github.com/aarnavt7/FORE-TRACE/releases/tag/v1.1.1
- Artifact: https://github.com/aarnavt7/FORE-TRACE/releases/download/v1.1.1/FORE_TRACE_artifact-v1.1.1.zip
- SHA-256: `94565338953d2eb5908766b53d45e1066dbef28bb9b82fb6bd534476a151d9c6`
- Size: `42,784,856` bytes
- External manifest SHA-256: `b64de1ddf6d999e43d8f4cec65db9d055b52e8bc2f2d7443bbf50aa4f3a6ef25`

The final paper PDF listed above is a separate release asset and is not part of the canonical reviewer-artifact ZIP.

Version 1.1.1 is solely a packaging repair that declares and lock-binds Matplotlib 3.11.1. It does not change retained scientific or display bytes, records, protocol, conclusions, privacy boundaries, or analytic-unit accounting. The unpublished v1.1.0 candidate is intentionally not provided.

## Reproduction boundary

The artifact is synthetic-only and contains no participant or private-draft data. Verification is model-free retained-record recomputation, not a new experiment. No model, encoder, or external API calls are required by the documented verification path.

After extracting the canonical ZIP into an empty directory, create the exact locked environment:

```bash
uv sync --locked --all-extras --python 3.13.9
```

Run the canonical one-command verification wrapper:

```bash
make reproduce-v1.1
```

The wrapper verifies the package and recomputes the retained records. The equivalent expanded workflow separates retained-result recomputation from exact paper-asset regeneration:

```bash
make reproduce-main
make regenerate-assets-v1.1
```

See the packaged `README.md`, `REPRODUCIBILITY.md`, `DATA_CARD.md`, `RESOURCES_AND_ASSETS.md`, checksum ledger, and machine-readable manifest for the complete protocol and evidence boundaries.

## Optional developer test suite

The model-free commands above do not require Git metadata. Four provenance/runtime tests in the broader developer suite bind receipts to `git rev-parse HEAD`; a release ZIP deliberately has no `.git` directory. After verifying the pristine ZIP digest and manifest, initialize Git and commit the unchanged extracted tree before running the complete suite:

```bash
git init -b main
git add --all
git -c user.name='FORE TRACE verifier' -c user.email='noreply@example.invalid' commit -m 'Bind verified v1.1.1 bytes'
make check
```

In a pristine extraction, 108/112 tests pass and those four stop only because no Git `HEAD` exists; after committing all 209 exact extracted members, 112/112 pass. This is a VCS-context portability limitation, not a scientific-recomputation failure.

## Licensing

Original code and documentation are provided under the MIT License. Author-controlled synthetic fixtures and retained synthetic material are provided under CC BY 4.0 to the extent the applicable rightsholders hold the relevant rights. Third-party dependencies and model references remain governed by their upstream terms; model weights are not redistributed.
