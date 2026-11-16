<p align="center">
  <img src="img/header.png" alt="Donato Gómez — iOS Developer" />
</p>

<h3 align="center">iOS Developer · Swift · SwiftUI · Swift Concurrency · Clean Architecture</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Swift%206-FA7343?style=for-the-badge&logo=swift&logoColor=white" alt="Swift 6" />
  <img src="https://img.shields.io/badge/SwiftUI-007AFF?style=for-the-badge&logo=swift&logoColor=white" alt="SwiftUI" />
  <img src="https://img.shields.io/badge/Swift%20Concurrency-3A3A3C?style=for-the-badge&logo=swift&logoColor=white" alt="Swift Concurrency" />
  <img src="https://img.shields.io/badge/SwiftData-111111?style=for-the-badge&logo=apple&logoColor=white" alt="SwiftData" />
  <img src="https://img.shields.io/badge/Swift%20Testing-34C759?style=for-the-badge&logo=swift&logoColor=white" alt="Swift Testing" />
  <img src="https://img.shields.io/badge/Swift%20Package%20Manager-F05138?style=for-the-badge&logo=swift&logoColor=white" alt="Swift Package Manager" />
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" alt="GitHub Actions" />
  <img src="https://img.shields.io/badge/CarPlay-000000?style=for-the-badge&logo=apple&logoColor=white" alt="CarPlay" />
  <img src="https://img.shields.io/badge/watchOS-000000?style=for-the-badge&logo=apple&logoColor=white" alt="watchOS" />
</p>

I build native iOS apps in Swift and SwiftUI, and I can take one from an empty project to production on my own. [ZonaSalsa](https://apps.apple.com/us/app/zonasalsa/id6759666915), live on the App Store, is one I designed and built alone.

Behind that: 3+ years at NTT DATA on production apps for the Government of Andalusia, Ferrovial, PRISA (Los40), Renfe and Vodafone, and my own apps for iOS, watchOS and macOS.

<p align="center">
  <a href="https://www.donatogomez.dev">Website</a> •
  <a href="https://www.linkedin.com/in/donatogomez/">LinkedIn</a> •
  <a href="https://medium.com/@donatogomez">Medium</a>
</p>

## 💼 Experience

**iOS Developer · NTT DATA** (2022 – 2025)

- **Ferrovial** — the only iOS developer on a new internal incident-management app, from scratch to delivery in ~3 months. I defined the architecture and stack (SwiftUI, async/await) and the UX/UI design, later adopted by the Android version, and integrated authentication through the Salesforce SDK and the client's proprietary mapping system.
- **Carpeta Ciudadana (Government of Andalusia)** — I analysed the legacy app (~90% Objective-C; it did not build) and documented the deep-refactoring and rebuild alternatives in a technical report. The app was then rebuilt from scratch in SwiftUI with Clean Architecture and MVVM, and I was part of that team (v2.0, June 2024, rated 4.7★ on the App Store) and of its later releases.
- **Los40 (PRISA)** — rebuilt the app's main screen in SwiftUI together with another developer, using Clean Architecture + MVVM, async/await and REST APIs. Shipped in v7.0.
- **Renfe (dōcō) and Vodafone** — production bug fixing in large SwiftUI and UIKit codebases, plus some enhancements; on Vodafone's app I also wrote tests.

Stack: Swift, SwiftUI, UIKit, MVVM, Clean Architecture, async/await, REST, CocoaPods, Git, Scrum.

Earlier: native Android development (Java) in an international, English-speaking team in Belgium.

## 📱 Apps and projects

### 🎵 ZonaSalsa — on the App Store

The official app of a 24/7 salsa radio station. I designed, built and shipped it on my own (v1.0 in February 2026, v1.1 in April) and I maintain it. There are also Android and web versions.

<a href="https://apps.apple.com/us/app/zonasalsa/id6759666915">
  <img src="https://developer.apple.com/assets/elements/badges/download-on-the-app-store.svg" alt="Download ZonaSalsa on the App Store" height="48" />
</a>

- **Background live streaming** with `AVPlayer` and an `AVAudioSession` in `.playback`; the audio player is an actor that reports its state through an `AsyncStream`.
- **Works without the UI**: a `@MainActor @Observable` playback coordinator owns playback, metadata and history, so Siri (App Intents), CarPlay, the Lock Screen and Control Center (`MPNowPlayingInfoCenter`, `MPRemoteCommandCenter`) keep working even when no view exists.
- **Now playing** (artist, song, artwork) refreshed every 15 s from the streaming server's played-tracks endpoint, plus song history and sharing to Stories.
- **Architecture**: layered (App / Core / Domain / Features / Platform), MVVM with small use cases, and every system framework behind a protocol.
- **Quality**: Swift 6 language mode with strict concurrency and ~300 tests with Swift Testing. iOS 18+, Spanish and English.

### 📡 [SignalFlow](https://github.com/donatogomez/signal-flow) — public on GitHub

Offline-first IoT fleet-monitoring app for iOS 26 and watchOS. Clean Architecture across ~23 SPM modules whose boundaries are enforced in CI, SwiftData in a `ModelActor`, on-device Foundation Models, widgets, a Live Activity and an Apple Watch app. ~230 Swift Testing tests and GitHub Actions.

### 🎛️ [audio-inspector](https://github.com/donatogomez/audio-inspector) — macOS, in progress

Technical audio-file analysis tool for macOS. Modular SPM package, 19 ADRs, OpenSpec specifications and ~1,900 tests.

### 🧠 [Quizly](https://github.com/donatogomez/quizly) — public on GitHub

Imports quizzes from JSON and Markdown, stores them locally and runs them offline in reproducible sessions. Strict layered architecture with unidirectional dependencies, zero third-party dependencies, actor-based file I/O, schema migrations and a deterministic session engine. Swift 6 · SwiftUI · async/await + actors · Codable · XCTest.

### 🥁 Bachata Rhythm — finished, not yet published

Rhythm-training app for bachata: six tracks (güira, bongó, bass, two guitars and a counting voice) across the derecho, majao and mambo sections, with tempo control, an AVFoundation audio engine, VoiceOver support and a Spanish/English UI. Swift 6 with complete strict concurrency.

## 🛠️ How I work

- **Spec-driven, AI-assisted development** (OpenSpec, ADRs). I own the architecture and module boundaries, validate the specs and review every change before merging.
- **Tests and CI green** before anything is done, and the compiler as a safety net: Swift 6 strict concurrency and warnings as errors.

## ✍️ Writing

I write about modern Swift on [Medium](https://medium.com/@donatogomez):

- [Reactive Swift Without Combine or Rx](https://medium.com/@donatogomez/reactive-swift-without-combine-or-rx-a35a5ba31e08) · demo: [ReactiveSwift6Demo](https://github.com/donatogomez/ReactiveSwift6Demo)
- [Understanding @MainActor in SwiftUI: A Practical Guide for Swift 6](https://medium.com/@donatogomez/understanding-mainactor-in-swiftui-a-practical-guide-for-swift-6-69e657872ec5) · demo: [MainActorCounter](https://github.com/donatogomez/MainActorCounter)
- [Swift Is Not Just iOS — And Never Was](https://medium.com/@donatogomez/swift-beyond-the-apple-ecosystem-an-underused-language-b5f712ca0c90)

## 🧰 Stack

Swift · SwiftUI · Swift Concurrency (async/await, actors, Sendable) · MVVM · Clean Architecture · Swift Package Manager · URLSession / REST · SwiftData · Swift Testing · XCTest · Git · GitHub Actions · App Store Connect / TestFlight · AVFoundation · CarPlay · App Intents · WidgetKit · watchOS · Scrum

Languages: Spanish (native) · English (C1, professional working proficiency)

---

<p align="center">
  Building something on Apple platforms? <a href="https://www.linkedin.com/in/donatogomez/">Message me on LinkedIn</a>.
</p>
