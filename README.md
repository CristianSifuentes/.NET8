# What's New in .NET 8

## Table of Contents
- [Overview of .NET 8](#overview-of-net-8)
- [Key Features & Improvements](#key-features--improvements)
  - [Performance Enhancements](#performance-enhancements)
  - [Garbage Collection Improvements](#garbage-collection-improvements)
  - [System.Text.Json Serialization](#systemtextjson-serialization)
  - [Globalization for Mobile Apps](#globalization-for-mobile-apps)
  - [Source-Generated COM Interop](#source-generated-com-interop)
- [.NET Libraries Enhancements](#net-libraries-enhancements)
- [Observability Improvements](#observability-improvements)
- [.NET SDK Enhancements](#net-sdk-enhancements)
  - [CLI Template Improvements](#cli-template-improvements)
  - [Publish to a Container](#publish-to-a-container)
  - [Native AOT Support](#native-aot-support)
- [P/Invoke Source Generation](#pinvoke-source-generation)
- [Related Releases](#related-releases)
- [Conclusion](#conclusion)
- [Useful Links](#useful-links)

---

## Overview of .NET 8
.NET 8 is the **successor to .NET 7**, bringing **performance improvements, better developer experience, and long-term support (LTS) for three years**.

Key highlights of .NET 8:
- **Unified Framework**: Extends support across cloud, desktop, mobile, and IoT.
- **Improved Performance**: Optimized runtime and **faster execution**.
- **Enhanced Developer Productivity**: New language features and improved debugging.
- **Better Observability**: **Enhanced tracing and logging** for cloud-native applications.

---

##  Key Features & Improvements

### Performance Enhancements
Performance has been a key focus in .NET 8, with improvements including:
- **JIT Compilation Enhancements**: More efficient **loop optimizations and register allocations**.
- **ARM64 Performance Boosts**: Optimized for **modern processors**.
- **SIMD Improvements**: **AVX-512 support** for better vector operations.
- **Dynamic PGO (Profile-Guided Optimization)**: Enabled **by default** for a **15% average performance gain**.

For more details, see [Performance Improvements in .NET 8](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/).

### Garbage Collection Improvements
.NET 8 introduces **dynamic memory limit adjustments**, useful in cloud environments:
- **Call `GC.RefreshMemoryLimit()`** to **adjust memory usage dynamically**.
- Reduces **excess memory allocation** for **better cost efficiency**.

### System.Text.Json Serialization
.NET 8 improves **JSON serialization** in multiple ways:
- **Built-in support for additional types** (e.g., `Int128`, `Half`, `Memory<T>`).
- **Polymorphic Serialization for Interface Hierarchies**.
- **Read-only property deserialization**.
- **Performance optimizations for `JsonNode` APIs**.

For more details, visit [What's new in System.Text.Json in .NET 8](https://devblogs.microsoft.com/dotnet/whats-new-in-system-text-json-in-net-8/).

###  Globalization for Mobile Apps
.NET 8 introduces **Hybrid Globalization Mode**:
- Uses **smaller ICU bundles** for **better performance**.
- Suitable for **mobile apps needing localization**.

### Source-Generated COM Interop
.NET 8 introduces **a new source generator for COM interop**:
- **Reduces interop overhead**.
- Works **seamlessly with `LibraryImportAttribute`**.
- Improves **performance for native integrations**.

---

## .NET Libraries Enhancements
### **New Features in .NET Libraries**:
- **Improved Reflection APIs**: Now **supports function pointers**.
- **More Time APIs**: `TimeOnly` and `DateOnly` now have **microsecond and nanosecond support**.
- **Rate Limiting APIs**: Better **traffic control in applications**.
- **New Cryptography Features**: **SHA-3 support** added.

For more information, check [.NET 8 Library API improvements](https://devblogs.microsoft.com/dotnet/announcing-dotnet-8-api-improvements/).

---

## Observability Improvements
.NET 8 introduces **better observability tools**:
- **Enhanced `Activity.CurrentChanged` Event**.
- **Improved metrics collection** for cloud apps.

---

## .NET SDK Enhancements

### 🏗 CLI Template Improvements
- **Improved `dotnet new` Command**:
  - **Tab completion** for **templates and options**.
  - **New template constraints** for defining **allowed operating systems and hosts**.

###  Publish to a Container
- **Container Images**: Now a **built-in feature** of `dotnet publish`.
- **Support for multi-platform builds** with `--platform`.

### Native AOT Support
.NET 8 enhances **Native AOT (Ahead-of-Time) compilation**:
- **Better cross-platform compatibility** (now supports **macOS, Linux, Windows**).
- **Reduces app sizes by up to 50%**.
- **Native AOT for iOS and Android apps** (experimental).

For more details, visit [Native AOT in .NET 8](https://devblogs.microsoft.com/dotnet/native-aot-in-dotnet-8/).

---

##  P/Invoke Source Generation
.NET 8 includes **P/Invoke Source Generation**:
- **Reduces runtime overhead**.
- **Supports custom marshalling** for better **native interop**.

For more details, check [P/Invoke Improvements in .NET 8](https://devblogs.microsoft.com/dotnet/pinvoke-improvements-in-dotnet-8/).

---

## Related Releases
.NET 8 brings updates to multiple .NET components:

| Component        | Key Features |
|-----------------|--------------|
| **C# 12**       | Collection expressions, default parameters in lambdas |
| **F# 8**        | Simplified syntax and performance improvements |
| **.NET MAUI**   | More controls and better Windows support |
| **ASP.NET Core**| Faster HTTP performance, new authentication features |
| **EF Core 8.0** | JSON column support, lazy loading improvements |
| **Windows Forms** | DPI scaling fixes and accessibility improvements |
| **WPF**         | Performance and bug fixes |
| **Orleans 8.0** | Scalable distributed application improvements |
| **ML.NET**      | New text classification APIs |

For more details, see:
- [What's new in ASP.NET Core 8](https://devblogs.microsoft.com/aspnet/whats-new-in-aspnet-core-8/)
- [What's new in EF Core 8.0](https://devblogs.microsoft.com/dotnet/whats-new-in-ef-core-8/)

---

## Conclusion
.NET 8 is **a major step forward** in performance, developer experience, and cloud-native capabilities.

Key Takeaways:
 **Native AOT optimizations** for **faster app startup**.  
 **Improved JSON serialization** and **new time APIs**.  
 **Better performance with SIMD, JIT, and ARM64 optimizations**.  
 **Cloud-ready features like rate limiting and improved observability**.  

---

##  Useful Links
-  [Download .NET 8](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)
-  [C# 12 Features](https://devblogs.microsoft.com/dotnet/csharp-12/)
-  [ASP.NET Core 8 Updates](https://devblogs.microsoft.com/aspnet/whats-new-in-aspnet-core-8/)
-  [Performance Improvements in .NET 8](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/)

---
