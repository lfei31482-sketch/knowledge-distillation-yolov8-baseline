# knowledge-distillation-yolov8-baseline

A clean **YOLOv8 baseline** snapshot used as the reference point for knowledge-distillation experiments. Based on the official Ultralytics release **v8.3.171** ([AGPL-3.0](LICENSE)).

[中文说明](README.zh-CN.md)

## What this repo contains

- Standard Ultralytics YOLOv8 implementation and model configurations.
- Official installation / training / validation / prediction / export tooling.

**Intentionally excluded:** knowledge-distillation, MoE, or other experimental improvements; datasets, checkpoints, weights, and experiment results.

## Baseline training

```bash
pip install -e .
yolo detect train model=ultralytics/cfg/models/v8/yolov8m.yaml data=/path/to/dataset.yaml epochs=150 imgsz=640
```

See [BASELINE.md](BASELINE.md) for the full baseline definition and provenance, and the upstream [Ultralytics docs](https://docs.ultralytics.com/) for data formats and options.

## Related repo

- Improvement (MGD distillation): [knowledge-distillation-yolov8-improve](https://github.com/lfei31482-sketch/knowledge-distillation-yolov8-improve)

## Provenance

- Upstream source: [ultralytics/ultralytics](https://github.com/ultralytics/ultralytics)
- Baseline revision: `v8.3.171` (`afb4e53`)
- License: [AGPL-3.0](LICENSE)
