# 📱 Mobile Development Environment Setup  

## 🎯 Objective  
The goal of this task is to set up and test a React Native mobile development environment using **Expo Go**. Expo Go allows developers to test React Native applications directly on physical devices without requiring heavy emulators or simulators.  

---

## ✅ Requirements  
Before setting up Expo Go, ensure the following tools are already installed:  
- **Node.js (LTS version)**  
- **Visual Studio Code (VS Code)**  
- **Compatible Operating System** (macOS, Linux, or Windows)  
- **Expo Go** on your physical device (Android or iOS)  

---

## 🚀 Why Expo Go?  
Unlike traditional mobile development that requires emulators (resource-heavy and costly to maintain), Expo Go allows you to:  
- Run your app directly on a **real device** (Android or iOS).  
- Avoid dealing with multiple hardware requirements (e.g., iPhone 7 → iPhone 16 Pro Max).  
- Save time with **instant testing** via QR code scanning.  
- Develop and test seamlessly across platforms.  

---

## 📥 Steps to Install Expo Go  

1. Visit the official Expo Go page: 👉 [https://expo.dev/go](https://expo.dev/go)  
2. Select the latest SDK version.  
3. Install Expo Go on your device:  
   - **Android** → [Google Play Store](https://play.google.com/store/apps/details?id=host.exp.exponent)  
   - **iOS** → [Apple App Store](https://apps.apple.com/app/expo-go/id982107779)  
4. Open the **Expo Go app** on your device.  
5. Create a new **Expo account** or log in with an existing account.  

---

## 📝 Setup Process & Challenges  

### My Setup  
- Installed Expo Go from the **Google Play Store / Apple App Store**.  
- Logged into my Expo account successfully.  
- Verified app is ready to scan QR codes for future React Native projects.  

### Challenges Faced  
- _(Example: Had issues with Expo Go login, fixed by resetting password.)_  
- _(Example: Network issues delayed installation, solved by switching to WiFi.)_  

---

## 📂 Repository Structure  

prodev-mobile-setup/

└── mobile-development-setup/

└── README.md


---

## ✅ Next Steps  
With Expo Go installed and working:  
- Future React Native projects can be run instantly on my phone.  
- Development will be smoother without needing heavy emulators.  


# First Mobile App with Expo

## Objective
The goal of this task is to set up and scaffold my first mobile app using the **Expo Router template**, make a small modification, run and test the app on my device, and then document the reset behavior.

---

## Steps Followed

### 1. Navigate to Project Directory

cd prodev-mobile-setup


### 2. Initialize Project with Expo Router

I created a new Expo project using the latest router template:


npx create-expo-app@latest .


This generated a project structure with `app/`, `constants/`, and configuration files.

### 3. Modify Home Screen

I opened the file:


app/(tabs)/index.tsx


* Located the default text: `Welcome!`
* Changed it to:


<Text style={styles.title}>First App Created</Text>


### 4. Run and Test the App

Started the development server:


npx expo start


* On **iOS**: scanned the QR code using the Camera app.
* On **Android**: scanned the QR code with the Expo Go app.

This successfully launched the app on my phone showing **First App Created**.

### 5. Reset the Project

I ran the reset command:


npm run reset-project


---

## Observations from Reset

* The `node_modules/` folder was deleted and reinstalled.
* The `.expo/` cache was cleared.
* It reset project dependencies, cleaning any changes to cached builds.
* After reset, the app still ran correctly but required reinstalling packages if any were missing.

---

## Project Structure (Key Files)

prodev-mobile-setup/
│
├── prodev-mobile-app-0x00/
│   ├── README.md
│   ├── app-example/
│   │   ├── app/
│   │   │   └── (tabs)/
│   │   │       └── index.tsx   <-- Edited "Welcome!" → "First App Created"
│   │   ├── constants/
│   │   │   └── Colors.tsx
│   │   └── package.json
│   └── ...


---

## Conclusion

I successfully scaffolded my first mobile app with Expo, modified the home screen, tested it on a physical device, and confirmed how `reset-project` works.

Next steps: Explore adding new screens, components, and navigation.



