# knowledge-distillation-yolov8-baseline

知识蒸馏实验用的**干净 YOLOv8 基线**快照，作为改进方法的对照组。基于 Ultralytics 官方发布版 **v8.3.171**（[AGPL-3.0](LICENSE)）。

[English](README.md)

## 本仓库包含

- 标准 Ultralytics YOLOv8 实现与模型配置。
- 官方的安装、训练、验证、预测、导出工具链。

**有意不包含：** 知识蒸馏、MoE 等实验性改进；数据集、权重、checkpoint 与实验结果。

## 基线训练

```bash
pip install -e .
yolo detect train model=ultralytics/cfg/models/v8/yolov8m.yaml data=/path/to/dataset.yaml epochs=150 imgsz=640
```

基线的完整定义与来源见 [BASELINE.md](BASELINE.md)；数据格式等细节见 [Ultralytics 官方文档](https://docs.ultralytics.com/zh/)。

## 相关仓库

- 改进方法（MoE 蒸馏、Dense Gate）：[knowledge-distillation-yolov8-improve](https://github.com/lfei31482-sketch/knowledge-distillation-yolov8-improve)

## 来源

- 上游代码：[ultralytics/ultralytics](https://github.com/ultralytics/ultralytics)
- 基线版本：`v8.3.171`（`afb4e53`）
- 许可证：[AGPL-3.0](LICENSE)
