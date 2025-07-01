# TarentoTestApp

This project is a **UI Test Sample** developed to demonstrate layout structuring and circular view placement using traditional XML-based Android UI.

---

## 🧪 Project Overview

The screen layout is divided vertically into two sections:

- 🔷 **Upper Layout**: Takes up 70% of the screen height  
- 🔶 **Lower Layout**: Takes up the remaining 30%  
- ⭕ **Circular View**: Intersects both layouts visually at their center boundary

This behavior was designed as per an interviewer’s request and implemented using standard Android **ConstraintLayout**.

---

## ⚙️ Technical Approach

- **ConstraintLayout** is used to define the `upper_layout` and `lower_layout` with `layout_constraintVertical_weight`.
- The **circular intersection view** is implemented as a customizable component — it can be:
  - A `View`
  - An `ImageView`
  - A `Button`
  - A `FloatingActionButton` (FAB)

You can freely replace these elements with **`FrameLayout`**, `RelativeLayout`, or basic `View` containers based on design requirements.

---

## 🧱 Architecture

This project follows the **MVVM pattern** and is structured according to **Clean Architecture** principles:

- `presentation` layer contains the **Home screen UI**
- XML is used for layout implementation to match the interview requirements

---

## 🧩 Jetpack Compose Alternative

The same layout can be reimagined using **Jetpack Compose**:

- `UpperLayout()` and `LowerLayout()` can be implemented as two composable functions
- A third optional `CircularOverlay()` can be created to simulate or replace the circular intersection view
- You can also embed the XML circular view inside Compose using `AndroidView`

---

## 📁 Modules & Layers

com.example.tarentotestapp
│
├── presentation
│ └── screens
│ └── home
│ └── HomeActivity.kt
│
└── res
├── layout
├── drawable
└── values

![Screenshot_20250701_215131](https://github.com/user-attachments/assets/be7e0cb7-6373-47d5-8b8c-ea006a7e484f)

<img width="348" alt="Screenshot 2025-07-01 at 10 09 21 PM" src="https://github.com/user-attachments/assets/0c035eac-1adf-44c6-bd00-82427b2de2d0" />

