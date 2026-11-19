# LeafScan — Plant Leaf Disease Detector

Upload a photo of a plant leaf and LeafScan identifies the crop and any disease, entirely in the browser with TensorFlow.js. Photos never leave the device.

**Live site:** https://pranav110507.github.io/leafscan/

- **38 classes:** 26 diseases across 14 crops, plus 12 healthy classes
- **Crops:** Apple, Blueberry, Cherry, Corn, Grape, Orange, Peach, Bell Pepper, Potato, Raspberry, Soybean, Squash, Strawberry, Tomato
- **Model:** MobileNetV2 (ImageNet) + classification head trained on the PlantVillage dataset with augmentation
- **Accuracy:** 96.2% top-1, 99.7% top-3 on 3,192 held-out test images

Model weights are stored as base64 text shards in `model/` and loaded from memory.

LeafScan is a decision-support tool, not a lab diagnosis. Dataset: PlantVillage (Hughes & Salathé, 2015).
