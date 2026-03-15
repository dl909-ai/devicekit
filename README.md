# 📱 Device Optimization Project

We use [DeviceKit](https://github.com/devicekit/DeviceKit) to detect and optimize for 2026 hardware (iPhone 17e, M5 iPads).

## 🚀 Supported Hardware
- **iPhone 17e:** Custom display scaling.
- **M5 iPad Pro (11" & 13"):** High-performance rendering mode.

## 🛠 Implementation
The logic is placed in `AppDelegate.swift`:

```swift
import DeviceKit

let device = Device.current

if device == .iPhone17e {
    print("Applying iPhone 17e display profile...")
} else if device.isOneOf([.iPadPro11M5, .iPadPro13M5]) {
    print("Activating M5 High-Performance mode.")
}


```swift
import DeviceKit

let device = Device.current

if device == .iPhone17e {
    print("Applying iPhone 17e display profile...")
} else if device.isOneOf([.iPadPro11M5, .iPadPro13M5]) {
    print("Activating M5 High-Performance mode.")
}
