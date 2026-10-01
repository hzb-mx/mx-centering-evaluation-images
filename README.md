# MX centring evaluation images

This repository contains the 1,334 original images used for a frozen comparison of two automated sample-centring proposals: Murko and ai-center.

The set is **not limited to BL14.1**. It combines curated Murko test samples with camera snapshots collected from multiple sources. It is shared to support inspection and independent evaluation of centring behaviour.

## Contents

- `images/` contains the original camera/test images, preserving the frozen source-relative layout.
- `manifest.json` lists each included image with byte and pixel SHA-256 checksums, dimensions, and source grouping.

The evaluation predictions, overlays, human-review data, trained model weights, and beamline-control software are intentionally not included.

## Scope and limitations

These images have no universal ground-truth click coordinates. They should therefore be used to assess proposed centring points visually or with separately supplied annotations, rather than as an accuracy-labelled training set. Source-specific camera geometry and acquisition metadata are incomplete for many images.

The repository records the frozen input set only. It does not make any claim about production readiness or control-system integration.

## Reproducibility

The manifest was derived from the frozen evaluation input inventory. Image bytes and decoded pixel hashes can be verified against `manifest.json`.

## Use

Please retain this README and the manifest with redistributed copies. Contact the repository maintainers before using the images for model training or any public redistribution.
