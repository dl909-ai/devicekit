### 📱 Device Optimization
We use [DeviceKit](https://github.com/devicekit/DeviceKit) to detect 2026 hardware (iPhone 17e, M5 iPads). 

**Configuration Steps:**
1. logic is placed in `AppDelegate.swift`.
2. It initializes `Device.current` to determine the model.
3. It sets global flags for Pro-Motion (120Hz) and M5 rendering pipelines.
