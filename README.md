# Contacts Content Provider – Android Application

## 📌 Project Overview

The **Contacts Content Provider** is a simple Android application developed using **Kotlin and XML** in Android Studio. It demonstrates data sharing in Android by accessing contact information through the built-in Contacts Content Provider.

The application retrieves contact names and phone numbers from the device and displays them on the screen after obtaining the user's permission.

## 🎯 Aim

To implement data sharing in Android using the Contacts Content Provider and display contact names and phone numbers using Kotlin.

## ✨ Features

- Display contact names and phone numbers.
- Access device contacts using the Android Contacts Content Provider.
- Request runtime permission to read contacts.
- Display contacts in a scrollable view.
- Handle permission denial and empty contact lists.
- Simple and user-friendly interface.

## 🛠️ Technologies Used

- **IDE:** Android Studio
- **Programming Language:** Kotlin
- **UI Design:** XML
- **Platform:** Android
- **Android API:** Contacts Content Provider
- **Permission:** `READ_CONTACTS`

## 📂 Project Structure

```text
ContactsProviderDemo/
│
├── app/
│   └── src/
│       └── main/
│           ├── java/
│           │   └── com/example/contactsproviderdemo/
│           │       └── MainActivity.kt
│           │
│           ├── res/
│           │   └── layout/
│           │       └── activity_main.xml
│           │
│           └── AndroidManifest.xml
│
├── README.md
└── build.gradle.kts
```

*Note: Your actual project may contain additional Gradle files, resource folders, and configuration files.*

## ⚙️ Requirements

- Android Studio installed on your computer.
- Android SDK configured in Android Studio.
- An Android emulator or a physical Android device.
- A device containing contacts with phone numbers for testing.

## 🚀 Installation and Execution

### Step 1: Clone the Repository

Open a terminal and run:

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Replace `YOUR_GITHUB_REPOSITORY_URL` with your actual GitHub repository URL.

### Step 2: Open the Project

1. Open Android Studio.
2. Select **Open**.
3. Choose the downloaded project folder.
4. Wait for Gradle synchronization to complete.

### Step 3: Run the Application

1. Connect an Android device or start an emulator.
2. Select the device in Android Studio.
3. Click the **Run ▶** button.
4. Wait for the application to launch.

### Step 4: Grant Permission

1. Click the **Display Contacts** button.
2. When prompted, allow the application to access contacts.
3. The available contact names and phone numbers will be displayed.

## 🔐 Android Permission

The application requires permission to read device contacts.

Add the following permission to `AndroidManifest.xml`, outside the `<application>` tag:

```xml
<uses-permission
    android:name="android.permission.READ_CONTACTS" />
```

The application also requests runtime permission before accessing the contacts.

**Privacy note:** Contact information is personal data. This application reads contacts for demonstration purposes and should not share or upload them without the user's informed consent.

## 🔄 Working Principle

1. The user opens the application.
2. The user clicks the **Display Contacts** button.
3. The application checks whether contact permission has been granted.
4. If permission is not granted, Android displays a permission request.
5. The `ContentResolver` queries the Contacts Content Provider.
6. A `Cursor` reads the contact names and phone numbers.
7. The retrieved details are displayed in a `TextView`.

## 🧩 Important Components

| Component | Purpose |
|---|---|
| `MainActivity.kt` | Handles application logic and user interactions. |
| `activity_main.xml` | Defines the user interface. |
| `AndroidManifest.xml` | Declares the required contacts permission. |
| `ContentResolver` | Queries the Contacts Content Provider. |
| `ContactsContract` | Provides constants and URIs for accessing contacts. |
| `Cursor` | Reads records returned by the query. |
| `READ_CONTACTS` | Allows the application to request access to contacts. |

## 📱 Expected Output

When the user clicks **Display Contacts** and grants permission, the application displays contacts in this format:

```text
Contacts Content Provider

[Display Contacts]

Name: Arun
Phone: 9876543210

Name: Priya
Phone: 9123456780
```

*The names and numbers above are examples. Actual output depends on the contacts stored on the device.*

## 🧪 Test Cases

| Test Case | Expected Result |
|---|---|
| Launch the application | Main screen appears. |
| Click Display Contacts | Permission is requested if needed. |
| Grant permission | Contacts are displayed. |
| Deny permission | A permission-denied message appears. |
| No contacts with phone numbers | An appropriate message is displayed. |

## 📚 Learning Outcomes

By completing this project, you will learn:

- The concept of data sharing in Android.
- How Android Content Providers work.
- How to use `ContentResolver` and `ContactsContract`.
- How to request runtime permissions.
- How to retrieve and display data using a `Cursor`.
- How to build a simple Android application using Kotlin and XML.

## 🔮 Future Enhancements

- Search contacts by name.
- Display contact profile images.
- Open contact details when an item is selected.
- Add a RecyclerView for a better contact list interface.
- Add contact filtering and sorting options.

## 👨‍💻 Author

**Your Name**

- GitHub: [Your GitHub Profile](https://github.com/)
- Project: Contacts Content Provider – Android Application

## 📄 License

This project is intended for educational and academic purposes. You may adapt it for learning and demonstration, subject to the applicable licenses of its dependencies.

## ✅ Result

The Android application demonstrates data sharing through the Contacts Content Provider by retrieving and displaying contact names and phone numbers after obtaining the required permission.
