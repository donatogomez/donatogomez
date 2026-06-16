<p align="center">
  <img src="img/header.png" alt="Donato Gómez — Apple Platforms Developer" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Swift%206-FA7343?style=for-the-badge&logo=swift&logoColor=white" />
  <img src="https://img.shields.io/badge/SwiftUI-007AFF?style=for-the-badge&logo=swift&logoColor=white" />
  <img src="https://img.shields.io/badge/SwiftData-111111?style=for-the-badge&logo=apple&logoColor=white" />
  <img src="https://img.shields.io/badge/Async%2FAwait-3A3A3C?style=for-the-badge&logo=apple&logoColor=white" />
  <img src="https://img.shields.io/badge/Actors-3A3A3C?style=for-the-badge&logo=apple&logoColor=white" />
  <img src="https://img.shields.io/badge/Swift%20Testing-34C759?style=for-the-badge&logo=swift&logoColor=white" />
  <img src="https://img.shields.io/badge/Xcode-0D96F6?style=for-the-badge&logo=xcode&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" />
  <img src="https://img.shields.io/badge/Fastlane-1FAA59?style=for-the-badge&logo=fastlane&logoColor=white" />
  <img src="https://img.shields.io/badge/TestFlight-007AFF?style=for-the-badge&logo=apple&logoColor=white" />
  <img src="https://img.shields.io/badge/CarPlay-000000?style=for-the-badge&logo=apple&logoColor=white" />
  <img src="https://img.shields.io/badge/DocC-0A84FF?style=for-the-badge&logo=apple&logoColor=white" />
  <img src="https://img.shields.io/badge/AI--Assisted%20Dev-10A37F?style=for-the-badge&logo=openai&logoColor=white" />
</p>

Apple platforms developer focused on building production-grade SwiftUI apps with clean architecture and real-world constraints.
I ship features end-to-end: API integration, persistence, CarPlay, TestFlight and App Store delivery.

<p align="center">
  <a href="https://donatogomez.dev">Website</a> •
  <a href="https://www.linkedin.com/in/donatogomez/">LinkedIn</a> •
  <a href="https://github.com/donatogomez">GitHub</a> •
  <a href="https://medium.com/@donatogomez88">Medium</a>
</p>

## 🚀 What I build

I specialize in native Apple apps using modern Swift (Swift 6 + SwiftUI), with a strong focus on:

- Clean Architecture & MVVM
- Unidirectional data flow
- Async/Await & Actors (strict concurrency)
- SwiftData persistence
- Audio streaming & CarPlay
- End-to-end delivery (Xcode Cloud, TestFlight)

## 📱 Apps

**🎵 Zona Salsa Radio** — Official app of the ZonaSalsa station. Live 24/7 salsa streaming with CarPlay, Lock Screen & Control Center, real-time now-playing, song history and light/dark themes. Built with Swift 6 + SwiftUI and AVPlayer/AVFoundation.

<a href="https://apps.apple.com/us/app/zonasalsa/id6759666915">
  <img src="https://developer.apple.com/assets/elements/badges/download-on-the-app-store.svg" alt="Download Zona Salsa Radio on the App Store" height="52" />
</a>

**🥁 Bachata Rhythm** — Educational rhythm-training app: 7 instruments, 5 sections, BPM control, AVFoundation audio engine, VoiceOver support and bilingual UI.

<img src="https://img.shields.io/badge/App%20Store-Coming%20Soon-8E8E93?style=for-the-badge&logo=apple&logoColor=white" alt="Bachata Rhythm — Coming Soon" />

**🧠 Quizly** — Native iOS app to import quizzes from multiple formats (JSON, Markdown), store them locally and solve them offline through dynamic, reproducible sessions. Strict layered architecture with unidirectional dependencies, zero third-party dependencies, actor-based file I/O, schema migrations and a deterministic session engine. Swift 6 · SwiftUI · async/await + actors · Codable · XCTest.

<a href="https://github.com/donatogomez/quizly">
  <img src="https://img.shields.io/badge/View%20Source-181717?style=for-the-badge&logo=github&logoColor=white" alt="Quizly source on GitHub" />
</a>

## ⚙️ Engineering notes — Zona Salsa Radio

A small, native, privacy-first app (no data collection, ~3.6 MB) with more going on under the hood than a typical radio player:

- **Live streaming** with `AVPlayer` over a remote audio stream, with a configured `AVAudioSession` (`.playback`) for uninterrupted background audio.
- **Lock Screen & Control Center** integration via `MPNowPlayingInfoCenter` and `MPRemoteCommandCenter`, keeping play/pause and metadata in sync with playback state.
- **CarPlay** support so the stream is controllable from the car.
- **Real-time now-playing** (artist / song / album) and song history.
- **Theming** (light / dark / automatic) and social sharing with per-destination flows (Instagram & Facebook Stories vs. generic share).
- **Architecture**: Clean Architecture + MVVM with unidirectional data flow; concurrency handled with `async/await` and actors.
- **Delivery**: shipped and maintained through Xcode Cloud → TestFlight → App Store.

> _Note: adjust the metadata source (ICY stream metadata vs. API polling) and any specifics to match the real implementation before publishing._

## ✍️ Writing

I write about modern Swift on [Medium](https://medium.com/@donatogomez88) — Swift 6, strict concurrency and SwiftUI architecture.

- [Reactive Swift Without Combine or Rx](https://medium.com/@donatogomez88/reactive-swift-without-combine-or-rx-a35a5ba31e08)
- [Understanding @MainActor in SwiftUI: A Practical Guide for Swift 6](https://medium.com/@donatogomez88/understanding-mainactor-in-swiftui-a-practical-guide-for-swift-6-69e657872ec5)
- [Swift Beyond the Apple Ecosystem: An Underused Language](https://medium.com/@donatogomez88/swift-beyond-the-apple-ecosystem-an-underused-language-b5f712ca0c90)

## 🧠 Developer Profile

```swift
struct DeveloperProfile {
    let name = "Donato Gómez"
    let role = "Apple Platforms Developer"

    let platforms = ["iOS", "iPadOS"]

    let architecture = [
        "MVVM",
        "Clean Architecture",
        "Unidirectional Data Flow"
    ]

    let coreTechnologies = [
        "SwiftUI",
        "SwiftData",
        "Async/Await",
        "Actors",
        "URLSession",
        "DocC",
        "Swift Testing"
    ]

    let principles = [
        "Clean Code",
        "Modular Architecture",
        "Performance Optimization",
        "Human-centered UI/UX",
        "Accessibility by default",
        "Developer Experience"
    ]

    let goals = [
        "Build maintainable Apple platform apps",
        "Apply Swift 6 strict concurrency in real products",
        "Ship production features end-to-end",
        "Grow through building, teaching and mentoring"
    ]
}
```

## 🧰 Core Stack

Swift 6 • SwiftUI • SwiftData • Async/Await • Actors • Xcode • Git • TestFlight

## 📈 GitHub Activity

<p align="center">
  <img src="https://streak-stats.demolab.com?user=donatogomez&theme=tokyonight" alt="GitHub streak stats" />
</p>
