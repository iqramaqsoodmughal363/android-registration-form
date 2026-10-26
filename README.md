# 📝 Android Registration Form

<p align="center">
  <b>A modern, validated registration form application for Android.</b>
</p>

<p align="center">
  <em>"A beautifully designed Android application built in Java featuring robust form validation, password masking, and a dynamic summary screen."</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Made%20with-%E2%9D%A4%EF%B8%8F-red" alt="Made with Love">
  <img src="https://img.shields.io/badge/Platform-Android-green" alt="Platform">
  <img src="https://img.shields.io/badge/Language-Java-orange" alt="Language">
  <img src="https://img.shields.io/badge/UI-Custom%20Layout-blue" alt="UI">
  <img src="https://img.shields.io/badge/Status-Complete-success" alt="Status">
</p>

---

## 📋 Overview

**Android Registration Form** is a clean, user-friendly application designed to demonstrate how to build and validate complex forms on the Android platform. Built entirely in **Java**, this app collects user data (Name, Email, Password, Phone, DOB, Gender, Country), validates the inputs, and displays a secure, formatted summary.

It showcases best practices for handling user input, customizing UI components, and securing sensitive data like passwords.

---

## ✨ Key Features

* **🚀 Splash Screen (`SplashActivity.java`):** A welcoming startup screen before the main form appears.
* **✅ Input Validation:** Ensures all required fields are filled correctly (e.g., valid email, non-empty fields).
* **🔒 Password Masking:** The user's password is securely hidden (converted to `***`) in the registration summary for privacy.
* **📋 Dynamic Summary:** Instantly generates and displays a clean summary of all entered details.
* **🎨 Custom UI Elements:** Features custom background drawables (`edittext_bg.xml`) and a dedicated image (`laptopgirl.jpg`) for an enhanced aesthetic.
* **📱 Responsive Layout:** Built with XML layouts that adapt well to different screen sizes.

---

## 🛠️ Tech Stack

| Category | Tools / Technologies |
|---|---|
| **Language** | Java |
| **IDE** | Android Studio |
| **UI Components** | XML Layouts, EditText, RadioButtons, Spinners |
| **Validation** | Custom Java Logic (String validation, Regex for email) |
| **Styling** | Custom Drawables (`edittext_bg.xml`) |

---

## 📂 Project Structure

```text
android-registration-form/
│
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/widgets/
│   │   │   │   ├── MainActivity.java        # Form logic & validation
│   │   │   │   └── SplashActivity.java      # App startup screen
│   │   │   ├── res/
│   │   │   │   ├── drawable/                # Custom assets
│   │   │   │   │   ├── edittext_bg.xml      # Custom input field background
│   │   │   │   │   ├── ic_launcher_background.xml
│   │   │   │   │   └── laptopgirl.jpg       # Header image
│   │   │   │   ├── layout/                  # UI Layouts
│   │   │   │   │   ├── activity_main.xml    # Main registration form
│   │   │   │   │   └── activity_splash.xml  # Splash screen layout
│   │   │   │   ├── mipmap-*/                # App launcher icons
│   │   │   │   └── values/                  # Colors, Strings, Themes
│   │   │   └── AndroidManifest.xml
│   │   └── build.gradle
│   ├── proguard-rules.pro
│   └── gradle/
├── build.gradle
├── settings.gradle
└── README.md
```

---

## 🚀 How to Build and Run

### Prerequisites
* **Android Studio** (Latest Version)
* **JDK 11** or higher
* **Android SDK** (API 21+)

### Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/iqramaaqsoodmughal363/android-registration-form.git
   ```
2. **Open in Android Studio**
   Open Android Studio → **File** → **Open** → Select the `Registration Form` folder.
3. **Sync Gradle**
   Wait for Gradle to sync. Click **"Sync Now"** if prompted.
4. **Build and Run**
   Connect your Android device or start an emulator, then click the **Run** button (green play icon).

---

## ⚙️ How It Works (Behind the Scenes)

### 1. The Registration Flow (`MainActivity.java`)
When the user clicks the "Register" button, the app gathers all inputs from the `EditText` fields. It then runs a series of `if` checks to validate the data. If any field is empty or invalid, a `Toast` message prompts the user to fix it.

### 2. Password Masking (`maskPassword` method)
For security, the app includes a custom `maskPassword` method. Instead of showing the raw password in the summary, it loops through the string and replaces every character with an asterisk `*`.

### 3. Dynamic Summary Generation
Once validated, the app builds a formatted `String` using `StringBuilder` or string concatenation. This summary is then displayed in a `TextView` (with `setVisibility(View.VISIBLE)`), instantly showing the user their submitted data.

---

## 🎯 Key Takeaways

* **Form Handling:** A perfect reference for handling multiple input types in Android.
* **Security Basics:** Demonstrates how to handle and mask sensitive data (passwords).
* **Custom UI:** Shows how to use custom XML drawables to make standard `EditText` views look beautiful.
* **Clean Logic:** Well-structured `if-else` logic for validating user input.

---

## 👩‍💻 Author

**Iqra Maqsood Mughal**

*Software Engineer · Full-Stack Developer · Code Craftsman · Android App Developer · Problem Solver 🚀*

```javascript
const codeIsLife = "Code is life";
while (true) { 
    learn(); 
    build(); 
    innovate(); 
}
```

---

## 📅 Date

October 26, 2026

---

## 📄 License

This project is intended for educational and personal use purposes.
