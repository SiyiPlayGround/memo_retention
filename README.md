
# Memory Retention App

A **privacy-first iOS app** for memory retention based on the **Ebbinghaus Forgetting Curve**.  
This app helps users memorize information through periodic reviews, using spaced repetition principles, and works completely offline.

---

## ✨ Features

- 📄 Create and manage memos with:
  - Title
  - Content
  - Tags
- 🔔 Auto-generate review schedules based on the **Forgetting Curve**:
  - Default intervals: 1, 2, 4, 7, 15, and 30 days (configurable)
- ⏰ Receive **local notifications** for review reminders (no network required)
- ✅ Mark memos as "Mastered" to stop review reminders
- 🔍 Search memos by title, content, and tags
- 📊 View review history and progress for each memo
- 🎨 Simple and clean SwiftUI interface

---

## 🛡️ Privacy Guarantee

- All data is stored **locally** using **Core Data**.
- No cloud syncing, no data collection, no analytics.
- App works 100% offline, without network permissions.

---

## 📂 Project Structure (MVVM + Repository Pattern)

```

MemoryRetentionApp/
├── CoreData/
│   ├── PersistenceController.swift
│   └── Memo.swift
├── Managers/
│   ├── NotificationManager.swift
│   └── ForgettingCurveManager.swift
├── Repositories/
│   └── MemoRepository.swift
├── ViewModels/
│   ├── MemoListViewModel.swift
│   └── ReviewViewModel.swift
├── Views/
│   ├── ContentView\.swift
│   ├── MemoListView\.swift
│   ├── MemoDetailView\.swift
│   ├── ReviewView\.swift
│   └── ReviewCardView\.swift
├── Models/
│   └── ReviewRecord.swift
├── MemoryRetentionApp.swift  (App entry point)
└── README.md

````

---

## 📋 Requirements

- Xcode 15+
- iOS 17+
- Swift 5.9+
- Supports both iPhone and iPad

---

## 🚀 Getting Started

1. Clone the repo:
```bash
git clone https://github.com/your-username/memory-retention-app.git
````

2. Open in Xcode:

```bash
open MemoryRetentionApp.xcodeproj
```

3. Build & Run on iOS Simulator or Device.

4. Grant Notification Permissions when prompted.

---

## 🔧 Customization

* To adjust review intervals, edit `ReviewScheduleConfig` in `ForgettingCurveManager.swift`:

```swift
var intervals: [Int] = [1, 2, 4, 7, 15, 30] // Days
```

---

## 📱 Screenshots

*(Add screenshots of your app here after running.)*

---

## 📄 License

MIT License. No commercial use without permission.

---

## 🤝 Contributions

Contributions, bug reports, and suggestions are welcome!

---

## ❤️ Acknowledgments

* Based on Ebbinghaus Forgetting Curve
* Powered by SwiftUI, Core Data, and UNUserNotificationCenter


