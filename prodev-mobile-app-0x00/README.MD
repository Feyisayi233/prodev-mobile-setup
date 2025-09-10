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

- Located the default text: `Welcome!`
- Changed it to:

<Text style={styles.title}>First App Created</Text>

### 4. Run and Test the App

Started the development server:

npx expo start

- On **iOS**: scanned the QR code using the Camera app.
- On **Android**: scanned the QR code with the Expo Go app.

This successfully launched the app on my phone showing **First App Created**.

### 5. Reset the Project

I ran the reset command:

npm run reset-project

---

## Observations from Reset

- The `node_modules/` folder was deleted and reinstalled.
- The `.expo/` cache was cleared.
- It reset project dependencies, cleaning any changes to cached builds.
- After reset, the app still ran correctly but required reinstalling packages if any were missing.

---

## Project Structure (Key Files)

prodev-mobile-setup/
│
├── prodev-mobile-app-0x00/
│ ├── README.md
│ ├── app-example/
│ │ ├── app/
│ │ │ └── (tabs)/
│ │ │ └── index.tsx <-- Edited "Welcome!" → "First App Created"
│ │ ├── constants/
│ │ │ └── Colors.tsx
│ │ └── package.json
│ └── ...

---

## Conclusion

I successfully scaffolded my first mobile app with Expo, modified the home screen, tested it on a physical device, and confirmed how `reset-project` works.

Next steps: Explore adding new screens, components, and navigation.
