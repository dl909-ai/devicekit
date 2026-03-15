# 📱 DeviceKit (2026 Hardware Fork)

A lightweight library to identify and optimize for Apple hardware, now updated for the 2026 product cycle.

## 🚀 2026 Hardware Support
This fork adds explicit support for the latest devices, allowing for custom UI scaling and performance modes.
- **iPhone 17e**
- **iPad Pro 11" (M5)**
- **iPad Pro 13" (M5)**

## 🛠 Implementation
To use these optimizations, call the detection logic in your `AppDelegate.swift`:

```swift
import DeviceKit

func application(_ application: UIApplication, didFinishLaunchingWithOptions ...) -> Bool {
    let device = Device.current

    if device == .iPhone17e {
        // Apply iPhone 17e specific layout
    } else if device.isOneOf([.iPadPro11M5, .iPadPro13M5]) {
        // Enable M5 High-Performance rendering
    }
    
    return true
}
