# 📱 Device Optimization Project

This repository uses [DeviceKit](https://github.com/devicekit/DeviceKit) to provide specific optimizations for the 2026 Apple hardware lineup.

## 🚀 Supported Hardware
- **iPhone 17e:** Custom display scaling.
- **M5 iPad Pro (11" & 13"):** High-performance rendering mode.

## 🛠 Implementation
The detection logic is housed in `AppDelegate.swift`:

```swift
import DeviceKit

let device = Device.current

if device == .iPhone17e {
    print("Applying iPhone 17e display profile...")
} else if device.isOneOf([.iPadPro11M5, .iPadPro13M5]) {
    print("Activating M5 High-Performance mode.")
}
