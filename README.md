# 🏋️ Fitness App

A comprehensive Flutter-based fitness application designed to help users track workouts, manage their diet, and stay fit with the help of AI-powered features.

## ✨ Features

Based on the modular architecture, the app includes the following key features:

-   **🔐 Authentication**: Secure user login and registration with token management.
-   **🏠 Home Dashboard**: Central hub for daily activity tracking and quick access to features.
-   **🏋️ Workouts & Exercises**: Detailed workout plans and exercise guides.
-   **🤖 Smart Coach / Chat with AI**: AI-powered assistant aimed at providing personalized fitness advice using Gemini.
-   **👤 Profile Management**: User settings, stats, and personal information.
-   **🏢 Gym Locator / Info**: Features related to gym lookup or details.
-   **🔒 Change Password**: Security settings for account management.
-   **🚀 Onboarding**: Smooth introduction flow for new users.

## 🛠️ Tech Stack & Architecture

This project is built using **Clean Architecture** principles and a robust tech stack:

-   **Framework**: [Flutter](https://flutter.dev/)
-   **State Management**: [Flutter Bloc](https://pub.dev/packages/flutter_bloc) (Cubit)
-   **Dependency Injection**: [GetIt](https://pub.dev/packages/get_it) & [Injectable](https://pub.dev/packages/injectable)
-   **Networking**: [Dio](https://pub.dev/packages/dio) for API requests with [Retrofit](https://pub.dev/packages/retrofit)
-   **Local Storage**: [Flutter Secure Storage](https://pub.dev/packages/flutter_secure_storage) & [Shared Preferences](https://pub.dev/packages/shared_preferences)
-   **AI Integration**: [Google Generative AI (Gemini)](https://pub.dev/packages/google_generative_ai)
-   **UI/UX**:
    -   `flutter_screenutil` for responsiveness.
    -   `shimmer` / `skeletonizer` for loading states.
    -   `flutter_svg` for vector graphics.
    -   `animated_text_kit` for animations.
    -   `google_fonts` for typography.
-   **Utilities**: `logger`, `equatable`, `intl`, `fluttertoast`.

## 📂 Project Structure

The project follows a feature-first approach:

```
lib/
├── core/            # Core utilities, networking, DI setup, common widgets
├── features/        # Feature modules
│   ├── auth/
│   ├── chat_with_ai/
│   ├── home/
│   ├── workouts/
│   ├── smart_coach/
│   └── ...
└── main.dart        # Entry point
```

## 🚀 Getting Started

### Prerequisites

-   Flutter SDK installed (Version ^3.9.2 recommended)
-   Dart SDK
-   Android Studio or VS Code

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/fitness_app.git
    cd fitness_app
    ```

2.  **Install dependencies:**
    ```bash
    flutter pub get
    ```

3.  **Run Code Generation (for Retrofit, Freeze, Injectable, etc.):**
    ```bash
    dart run build_runner build --delete-conflicting-outputs
    ```

4.  **Run the app:**
    ```bash
    flutter run
    ```

## 📸 Screenshots

*(Add your application screenshots here)*

| Home Screen | Workout Details | AI Chat |
|:-----------:|:---------------:|:-------:|
|   ![Home]   |    ![Workout]   | ![Chat] |

---

Made with ❤️ using Flutter
