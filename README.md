# Spectra-Pro: Advanced Mobile Security & Reverse Engineering Toolkit

![Spectra-Pro Banner](logo.svg)

**Spectra-Pro** is a professional-grade, high-performance platform designed for security researchers, reverse engineers, and mobile developers. It provides a unified environment to analyze, debug, and intercept Android application behavior in real-time by combining static analysis, dynamic instrumentation, smart security scanning and network interception into a single, sleek dashboard.

---

## 🚀 Key Features

### 1. Dynamic Analysis
Unleash the power of Frida with a streamlined instrumentation engine. Monitor and modify app behavior as it happens.

*   **Advanced Script Injection**: 
    *   **Attach**: Inject scripts into already running processes without interruption.
    *   **Spawn**: Launch applications with scripts pre-loaded to capture early startup behavior.
*   **Ready-to-Use Script Library**: Access a curated collection of pre-defined Frida scripts for common tasks (SSL bypass, Root detection bypass, API monitoring, etc.).
*   **Professional Script Editor**: Full-featured IDE powered by **Monaco Editor**, featuring:
    *   Syntax highlighting and auto-completion.
    *   Inline error detection.
    *   Script drafts and persistence.
*   **Real-Time Log Streamer**: Comprehensive log console with:
    *   Color-coded log levels (Info, Warning, Error).
    *   Advanced filtering and search.
    *   Exportable logs for later analysis.
*   **Workspaces (Projects)**: Organize your scripts and findings into persistent projects for different target applications.
*   **Dynamic Template Generation**: Instantly create hook templates for any class or method discovered during exploration.

### 2. Static Analysis
Deep-dive into the application's DNA. Decompile and analyze the code without running it.

*   **Multi-Format Decompilation**: Support for **APK, XAPK, APKM, and AAB (App Bundles)**. Seamlessly decompress and decompile to Java/Smali.
*   **Smart Security Scan**: Automated vulnerability scanner that identifies critical security flaws:
    *   Insecure Android Manifest configurations (exported components, debuggable flag).
    *   Weak cryptographic implementations.
    *   Hardcoded secrets and API keys.
*   **Smart Hot Objects**: Automated Hot Object scanning that identifies behaviour-related methods,fields,classes:
    *   Results show classes, methods, or fields associated with core logic, billing, authentication, or debugging.
    *   Navigate to the file directly from the results list.
    *   Create Frida hook script directly from the code.

*   **Smart App Intelligence**: 
    *   **SDK Detection**: Automatically identify third-party libraries and frameworks.
    *   **Endpoint Extraction**: Discover hidden API URLs and hardcoded IP addresses.
    *   **Native Library Analysis**: Inspect ELF headers and strings in packed `.so` files.
    *   **Deep Link Mapper**: Extract and visualize all supported URI schemes and hosts.
*   **Advanced Search Engine**: Perform global searches across thousands of files with case sensitivity and exact match options.
*   **Session Management**: Save and resume analysis sessions. Never lose your progress on complex decompilation tasks.
*   **Dynamic Integration**: Bridge the gap between static and dynamic analysis. Create Frida hooks directly from a class, method, or field in the source code viewer.
*   **Comprehensive Reporting**: Generate professional HTML and JSON reports with all findings, metrics, and evidence.

### 3. Proxy & HTTP Interception
A powerful MITM (Man-In-The-Middle) proxy designed specifically for mobile traffic.

*   **One-Click CA Installation**: Automated wizard to generate and install the Spectra CA certificate on the target device (supports Android 10+ and APEX overlays).
*   **Live Interceptor**: 
    *   Pause requests and responses on-the-fly.
    *   Modify headers, status codes, and body payloads before they reach their destination.
    *   Drop suspicious traffic instantly.
*   **SSL Pinning Bypass**: Built-in, automated logic to bypass certificate pinning for common libraries like OkHttp, Volley, and TrustManager.
*   **Advanced Data Viewers**: Support for multiple data encodings and formats:
    *   **Decompression**: Automatic decoding of Gzip, Deflate, Brotli (br), and Zstd.
    *   **Binary Tools**: Specialized viewers for Protobuf (InnerTube/YouTube) and other binary payloads.
*   **Full Request Metadata**: Detailed view of every interaction, including package name (via `x-requested-with`), timing, and server info.

### 4. General & Toolkit Management
A central hub for managing your research environment.

*   **Device Wizard & Connection**: A guided 5-step process to connect ADB, verify root access, and ensure device readiness.
*   **Frida Lifecycle Management**: 
    *   Automated detection of device architecture.
    *   One-click download, push, and deployment of compatible `frida-server` versions.
    *   Start/Stop/Reload server control.
*   **App Browser & Selector**: Filterable list of all installed user and system apps with icons and metadata.
*   **Component Browser**: Enumerate and interact with all Activities, Services, and Receivers within an app.
*   **Classes/Methods Explorer**: Live enumeration of loaded classes in a running process.
*   **Professional UI/UX**: 
    *   **Premium Themes**: Sleek, modern Dark and Light modes.
    *   **Interactive Design**: Micro-animations and real-time status indicators.
*   **System Event Logs**: Monitor background operations, ADB commands, and toolkit status in a dedicated event log.

---


## 📦 Getting Started

### Prerequisites
*   Windows 10/11
*   [Android Platform Tools (ADB)](https://developer.android.com/tools/releases/platform-tools)
*   [Java Runtime Environment (JRE) 17+](https://www.oracle.com/java/technologies/downloads/) (Required for JADX)
*   Rooted Android Device or Emulator
*   Install any version of Frida on your pc [Frida Installation Guide](https://frida.re/docs/installation/)

### Installation & Runnning
1.  Download the latest release from the [Releases](https://github.com/ahmaddarwesh/Spectra/releases) page.
2.  Run the installer executable.
3.  Request your free license for help us with testing from the [Main Tool Website](""https://spectra-pro-tool.web.app/)
4.  Activate your copy of the tool by paste the license key.
5.  Connect your Android device via USB or Wireless ADB.
6.  Launch Spectra-Pro and follow the **Device Wizard** to begin analysis. 
7.  Open Static-Analysis tool to start reverse engineering and advanced scanning.
8.  Open Proxy tool to start MITM attack with interceptor.

---
## Important Links 
* [Spectra-Pro Website](https://spectra-pro-tool.web.app/)
* [Spectra-Pro Youtube Channel](https://www.youtube.com/@spectra-tool)
---
*Built with ❤️ by the Spectra-Pro Team for Security Research.*
