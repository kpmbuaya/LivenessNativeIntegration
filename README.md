# Liveness Plugin Integration Guide

This repository provides a sample project demonstrating how to integrate the `liveness-plugin` with a Flutter native application using the `gateway` component.

## 📦 Repository Setup

To get started, clone and organize the following repositories:

### 1. Clone Required Repositories

- **Liveness Plugin**  
  - Clone the [`liveness-plugin`](https://github.com/KB-FMF/flutter-package-plugin-liveness/tree/feat/MCT-210-liveness-ios) repository:
  ```bash
  git clone https://github.com/KB-FMF/flutter-package-plugin-liveness.git
  ```
  - Rename the folder to **liveness-plugin**.
  - Switch to the branch configured for liveness integration (e.g., feat/MCT-210-liveness-ios). Avoid using the main branch unless it contains the latest setup.
    
- **Gateway**
  - Clone the [`gateway`](https://github.com/kpmbuaya/LivenessGateway) repository:
  ```bash
  git clone https://github.com/kpmbuaya/LivenessGateway.git
  ```
  - Rename the folder to **gateway**.

- **Sample Project**
  - Clone the [`sample project`](https://github.com/kpmbuaya/LivenessNativeIntegration) repository


### 2. LivenessGateway - Folder Structure - Mandatory
![Finder 2025-04-29 16 50 03](https://github.com/user-attachments/assets/350d6013-e599-44da-962c-6f4499ca7e85)
```bash
liveness/
├── gateway/
├── liveness-plugin/
└── LivenessNativeIntegration/
```

### 3. Setup Project 
- **Gateway**
  - Run
    ```bash
    flutter precache -iOS
    flutter clean
    flutter pub get
    cd .ios
    pod install
    ```
- **Sample Project**
  - Run
    ```
    pod install
    ```

# Output
## Debug Output
![Xcode-29 04 2025 at 17 08 55@2x](https://github.com/user-attachments/assets/50da4e78-51f8-4cc8-b461-7671b5065532)

## Result
https://github.com/user-attachments/assets/95571d14-d1ac-4957-b8ab-7797263d4fa1

## Warning on first-time app launch
![Xcode-29 04 2025 at 17 11 35@2x](https://github.com/user-attachments/assets/41131963-6441-4223-b145-040845af1c4b)

## Warning on first-time access to the liveness feature
![Xcode-29 04 2025 at 17 12 24@2x](https://github.com/user-attachments/assets/7058cd9e-de5c-4078-822c-386545726abe)

## This warning does not lead to any errors and is also present in the KPM project.
![Finder 2025-04-29 17 19 32](https://github.com/user-attachments/assets/e9bfd2f8-e036-49b5-88fa-aaa8dcb90c50)
