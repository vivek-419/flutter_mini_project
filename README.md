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

