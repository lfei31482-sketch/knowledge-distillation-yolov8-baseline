# YOLOv8 Baseline

This repository is a clean baseline snapshot for knowledge-distillation experiments. It is based on the official Ultralytics release **v8.3.171** and retains the upstream AGPL-3.0 license.

## Scope

Included:

- Standard Ultralytics YOLOv8 implementation and model configurations.
- Official installation, training, validation, prediction, and export tooling.

Intentionally excluded:

- Knowledge-distillation, MoE, or other experimental improvements.
- Datasets, annotations, checkpoints, model weights, experiment logs, and generated results.

## Baseline training

Install the package from the repository root:

```bash
pip install -e .
```

Train a standard YOLOv8m detector with your own dataset configuration:

```bash
yolo detect train model=ultralytics/cfg/models/v8/yolov8m.yaml data=/path/to/dataset.yaml epochs=150 imgsz=640
```

See the upstream [Ultralytics documentation](https://docs.ultralytics.com/) for data formats and additional options.

## Provenance

- Upstream source: [ultralytics/ultralytics](https://github.com/ultralytics/ultralytics)
- Baseline revision: `v8.3.171` (`afb4e53`)
- License: [AGPL-3.0](LICENSE)
