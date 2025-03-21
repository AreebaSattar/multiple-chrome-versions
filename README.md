# Installing Multiple Versions of Chrome on a Laptop

## Overview
This guide provides step-by-step instructions on how to install multiple versions of Google Chrome on a single laptop. By following this method, you can run older versions of Chrome independently without interfering with the main installation.

## Prerequisites
Before proceeding, ensure you have **7-Zip** installed on your laptop. This tool is required to extract files from the Chrome installer.

## Steps to Install an Older Chrome Version

### 1. Downloading an Older Version of Chrome
- Visit [Google Chrome Old Versions - Uptodown](https://google-chrome.en.uptodown.com/windows/versions) to download the desired version.
- Choose the required version (e.g., **127.0.6533.120**).
- Download the `.exe` file.

### 2. Extracting the Installer
- Use **7-Zip** to extract the downloaded `.exe` file.
- After extraction, you will find a file named `updater.zip`.
- Extract `updater.zip` to proceed further.

### 3. Locating the Chrome Installer
- Inside the extracted folder, navigate to the `bin` folder.
- Go to the `Offline` directory and move two steps forward.
- Locate the `127.0.6533.120_chrome_installer` file.

### 4. Extracting Chrome Files
- Use **7-Zip** to extract `127.0.6533.120_chrome_installer`.
- Inside the extracted files, locate `chrome.zip`.
- Extract `chrome.zip`, which contains a folder named **Chrome-bin**.

### 5. Creating a Folder for the Chrome Version
- Navigate to `C:\Program Files\Google\`.
- Create a new folder and name it based on the Chrome version (e.g., **Chrome127**).
- Inside **Chrome127**, create another folder named **Application**.

### 6. Copying Extracted Chrome Files
- Copy all files from **Chrome-bin** and paste them into:
  ```
  C:\Program Files\Google\Chrome127\Application
  ```

### 7. Creating a Shortcut for the Chrome Version
- Navigate to `C:\Program Files\Google\Chrome127\Application`.
- Right-click on `chrome.exe` and select **Create Shortcut**.
- Move the shortcut to your desired location (e.g., Desktop).

### 8. Modifying the Shortcut
- Right-click on the shortcut and select **Properties**.
- In the **Target** field, modify it by adding the following argument at the end:
  ```
  "C:\Program Files\Google\Chrome127\Application\chrome.exe" --user-data-dir="C:\ChromeTestProfile"
  ```
- You can replace `ChromeTestProfile` with any preferred folder name.

## Running the Installed Chrome Version
Now, when you open the modified shortcut, it will launch the specified Chrome version with a separate user profile.

## Additional Information
- Screenshots illustrating each step will be provided in the accompanying Word document.
- This method allows multiple Chrome versions to run independently without conflicting with the main Chrome installation.


