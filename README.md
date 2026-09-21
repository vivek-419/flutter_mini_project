# 🩺 My Health Tracker — Flutter Mobile Application

[![Flutter](https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-badge&logo=Flutter&logoColor=white)](https://flutter.dev)
[![Dart](https://img.shields.io/badge/dart-%230175C2.svg?style=for-the-badge&logo=dart&logoColor=white)](https://dart.dev)
[![Material Design 3](https://img.shields.io/badge/Material_3-7C4DFF?style=for-the-badge&logo=materialdesign&logoColor=white)](https://m3.material.io)
[![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](LICENSE)

A modern, responsive, offline-first Healthcare & Personal Wellness Flutter application built for mobile, tablet, and desktop platforms. Designed with Google's Material Design 3 guidelines, custom typography (**Poppins**), and a structured single-scaffold shell architecture.

---

## 📱 Application Screens & Features

| 👤 Patient Profile | 📊 Health Metrics Grid | 📝 Book Appointment | 💡 Health Tips |
| :---: | :---: | :---: | :---: |
| **Profile banner with overlapping avatar, personal vitals, and emergency alert cards.** | **2-column responsive grid displaying real-time vital indicators and stats.** | **Comprehensive interactive booking form with modal confirmation.** | **Curated daily wellness tips with interactive bookmarking.** |

### 🌟 Key Highlights
* **1. Patient Profile Screen**:
  - Layered header banner using `Stack` and `Positioned` for an overlapping avatar effect.
  - Quick-view personal information cards (Age, Gender, Blood Group).
  - Physical measurements with calculated BMI metrics.
  - Emergency medical alert card with contact info and allergy warnings.

* **2. Health Metrics Screen**:
  - Real-time vitals monitoring grid powered by `GridView.builder`.
  - Translucent color-coded cards for Heart Rate, Blood Pressure, Blood Sugar, Hydration, Steps, and Sleep.
  - Responsive flex layout with `Expanded` and `SliverGridDelegate`.

* **3. Doctor Appointment Booking Form**:
  - Text input handling with `TextField` and `TextEditingController`.
  - Department and specialist selection with `DropdownButton`.
  - In-Person vs. Online consultation selection via `RadioGroup` and `Radio`.
  - First-time visit `Checkbox` and SMS reminder `Switch`.
  - Interactive popup modal (`AlertDialog`) verifying booking details before submission.
  - Quick feedback notifications using `SnackBar`.

* **4. Daily Wellness & Tips Screen**:
  - Dynamic, memory-efficient list powered by `ListView.builder`.
  - Interactive favorite/bookmark system using `Set<int>` and dynamic `IconButton` state toggling.
  - Instant `SnackBar` toast alerts when saving or removing tips.

* **5. Navigation Shell**:
  - Global `AppBar` with dynamic title switching.
  - Side slide-out `Drawer` displaying profile details and emergency contact shortcuts.
  - Fixed 4-tab `BottomNavigationBar` switching active screens seamlessly.

---

## 🛠️ Tech Stack & Architecture

* **Framework**: [Flutter](https://flutter.dev) (v3.x / Dart 3.x)
* **Design System**: Material Design 3 (`useMaterial3: true`)
* **Typography**: Custom offline **Poppins** font family (Regular & Bold 700)
* **State Management**: Built-in declarative `StatefulWidget` & `setState()`
* **Data Layer**: Self-contained local Dart models (100% offline, zero backend dependency required)

---

## 📁 Project Structure

```
mini_project/
├── 📄 pubspec.yaml                 # Dependencies, assets, and Poppins font configuration
├── 📁 assets/                      # Local image assets (flower.jpg)
├── 📁 fonts/                       # Poppins font files (Poppins-Regular.ttf, Poppins-Bold.ttf)
└── 📁 lib/
    ├── 📄 main.dart                # App entry point, MaterialApp theme, Scaffold & Navigation
    ├── 📁 data/
    │   └── 📄 dummy_data.dart      # Static patient info, health metrics, tips, and doctor lists
    └── 📁 screens/
        ├── 📄 patient_details_screen.dart  # Screen 1: Profile & Vitals (Stack, Cards)
        ├── 📄 health_metrics_screen.dart   # Screen 2: 2x3 Vitals Grid (GridView.builder)
        ├── 📄 appointment_screen.dart      # Screen 3: Interactive Booking Form (Inputs, Dialog)
        └── 📄 health_tips_screen.dart      # Screen 4: Dynamic Tips List (ListView.builder, Favorites)
```

---

## 🧱 Widgets Showcase

This project demonstrates comprehensive mastery over essential Flutter widgets:

| Category | Widgets Used |
| :--- | :--- |
| **Structure & Shell** | `MaterialApp`, `Scaffold`, `AppBar`, `Drawer`, `DrawerHeader`, `BottomNavigationBar` |
| **Layout & Positioning** | `Stack`, `Positioned`, `Row`, `Column`, `Container`, `Padding`, `SizedBox`, `Expanded`, `SingleChildScrollView` |
| **Collections & Scrollables** | `ListView.builder`, `GridView.builder`, `SliverGridDelegateWithFixedCrossAxisCount` |
| **Form & Input Controls** | `TextField`, `TextEditingController`, `DropdownButton`, `RadioGroup`, `Radio`, `Checkbox`, `Switch` |
| **Buttons & Dialogs** | `ElevatedButton`, `TextButton`, `IconButton`, `AlertDialog`, `showDialog`, `SnackBar` |
| **Visual & UI Styling** | `Card`, `CircleAvatar`, `ClipRRect`, `Icon`, `Text`, `Divider`, `LinearGradient`, `BoxDecoration` |

---

## 🚀 Getting Started & Installation

### Prerequisites
- [Flutter SDK](https://docs.flutter.dev/get-started/install) installed on your machine.
- Android Studio / Xcode / VS Code with Flutter extension.
- Connected Android/iOS device, emulator, or Chrome browser.

### Run Locally

1. **Clone the repository**:
   ```bash
   git clone https://github.com/vivek-419/flutter-health-tracker.git
   cd flutter-health-tracker
   ```

2. **Install dependencies**:
   ```bash
   flutter pub get
   ```

3. **Run the application**:
   ```bash
   flutter run
   ```

---

## 👨‍💻 Author

**Vivek Addagatla**  
- GitHub: [@vivek-419](https://github.com/vivek-419)
- Academic Mini Project — Healthcare Flutter Application

---

## Screenshots
<img width="496" height="795" alt="Screenshot 2026-09-21 at 6 12 38 PM" src="https://github.com/user-attachments/assets/90893333-fef5-42a1-a64f-42bd66cd56eb" />

<img width="499" height="794" alt="Screenshot 2026-09-21 at 6 13 04 PM" src="https://github.com/user-attachments/assets/943fcfde-90ca-4414-8f7d-0aa886cbbacc" />

<img width="498" height="795" alt="Screenshot 2026-09-21 at 6 13 26 PM" src="https://github.com/user-attachments/assets/886d1d56-83c7-4ee7-a0ee-e6155528e951" />

<img width="492" height="792" alt="Screenshot 2026-09-21 at 6 13 54 PM" src="https://github.com/user-attachments/assets/d7e5f70e-32f2-4c5f-a4bb-874dca6a175b" />



