<!-- ===== HEADER ===== -->

<p align="center">
    <img src="./logo.svg" alt="WebBox Logo" height="80">
</p>

<h1 align="center">
    <strong>WebBox</strong> <span style="font-weight:300;">Projects</span>
    <br><br>
</h1>

<!-- ===== MAIN CONTENT ===== -->

## 🧱 WebBox Projects

### [webbox-runtime](https://github.com/webboxcore/webbox-runtime)
The core runtime written in Rust. It powers all WebBox Apps by launching isolated micro-VMs and rendering them in native system windows via WebView. This project is structured as a Rust workspace composed of multiple dedicated crates, each serving a distinct purpose.

**Notable Crates:**
- [`webbox-protocol`](https://github.com/webboxcore/webbox-runtime/tree/main/crates/webbox-protocol) – Defines interprocess and VM communication protocols.
- [`webbox-manager`](https://github.com/webboxcore/webbox-runtime/tree/main/crates/webbox-manager) – Controls lifecycle of WebBox Machines (VMs).
- [`webbox-builder`](https://github.com/webboxcore/webbox-runtime/tree/main/crates/webbox-builder) – Handles `.wapp` build and packaging tools.
- [`webbox-bundle`](https://github.com/webboxcore/webbox-runtime/tree/main/crates/webbox-bundle) – Manages the WebBox Bundle format.
- [`webbox-command`](https://github.com/webboxcore/webbox-runtime/tree/main/crates/webbox-command) – CLI interfaces for runtime operations.
- [`webbox-window`](https://github.com/webboxcore/webbox-runtime/tree/main/crates/webbox-window) – Native window abstraction backed by WebView.

The main binary, `webbox`, is located at the project root and compiles into the system executable (`webbox.exe`, etc.).

---

### [webbox-core](https://github.com/webboxcore/webbox-core)
A native-like GUI WebBox App used to manage installed apps, virtual machines, system settings, and access the WebBox Store. Runs on top of the WebBox Runtime.

---

### [webbox-platform](https://github.com/webboxcore/webbox-platform)
The Laravel backend that powers the entire WebBox ecosystem: account management, the WebBox Store, licensing, app publishing, telemetry, and other centralized platform services.

---

### [webbox-installer](https://github.com/webboxcore/webbox-installer)
Cross-platform native installers (for Windows, macOS, and Linux) that fetch the latest WebBox Runtime and guide users through initial setup using familiar OS-native installer wizards.

<!-- ===== FOOTER ===== -->

<h1 align="center" aria-hidden="true" role="presentation">&nbsp;</h1>

<p align="center">
    <small>
        Developed in Cornwall<br>
        &copy; Copyright 2025, Optical Raze Inc.
    </small>
</p>