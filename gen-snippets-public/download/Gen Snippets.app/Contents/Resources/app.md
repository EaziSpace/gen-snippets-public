# Basic Information
- **Project Name:** GenSnippets
- **Platform:** macOS
- **Minimum Deployment Target:** macOS 11.5 (Big Sur)
- **Xcode Version:** 16.2
- **Swift Version:** 5.0
- **Development Team ID:** GY8FNKSR7D

# Architecture & Frameworks
## UI Framework:
- **SwiftUI** as the main UI framework
- **AppKit** for some custom components (CustomTextEditor)

## System Frameworks:
- Foundation
- Carbon
- Cocoa
- AppKit

## System Permissions:
- Input Monitoring
- Accessibility
- Apple Events
- File Access (read-only)

# Key Features
1. **Text Expansion/Snippet Manager:**
   - Create and manage text snippets
   - Automatically replace text based on shortcuts
   - Local storage using UserDefaults

2. **Keyboard Monitoring:**
   - Monitor keyboard input
   - Handle dead keys and Unicode input
   - System-wide event tap

# Project Structure
## Views:
- ContentView (Main UI)
- ShortcutDetailView
- CustomTextEditor
- AddShortcutView
- SuccessView

## Models:
- Shortcut
- ShortcutDataManager
- TextExpander

## Supporting Files:
- Info.plist
- Entitlements
- Asset Catalog

# Technical Specifications
- Uses **MVVM pattern**
- **ObservableObject** for state management
- **Async/await** for asynchronous tasks
- **UserDefaults** for persistent storage
- **Notification Center** for internal communication

# Security & Privacy
- Requires the following permissions:
  - Input Monitoring
  - Accessibility
  - Apple Events
- **Sandbox enabled** with some exceptions

# Build Settings
- Optimized for Apple Silicon
- Sandbox enabled
- Automatic code signing
- Hardened runtime enabled
- Asset catalog compiler enabled for Swift

# Overview
This is a text content application for macOS, allowing users to create and manage text snippets. It features a modern UI built with SwiftUI and leverages system-wide functionalities through low-level macOS APIs.