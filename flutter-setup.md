# FLUTTER Setup

1. Create a folder `Android` at `C:\`.

2. Add `ANDROID_HOME` with value `C:\Android` in environment variables.

3. Download `cmdline-tools` from:  
   [Android Studio command-tools](https://developer.android.com/studio/#command-tools)

4. Extract the downloaded compressed folder contents to:  
   `C:\Android\cmdline-tools\latest\`

5. Run the following commands in terminal to install the corresponding packages:
   - Emulator
    ```bash
    sdkmanager emulator
    ```
   - Platform Tools
    ```bash
    sdkmanager platform-tools
    ```

6. Add the following paths to the **Environment Path Variables**:
   - `C:\Android\cmdline-tools\latest\bin`
   - `C:\Android\build-tools\x.x.x`
   - `C:\Android\emulator`
   - `C:\Android\platform-tools`

7. Download Flutter from the official website.

8. Extract the downloaded compressed folder contents to:  
   `C:\Android\flutter\`

9. Add `C:\Android\flutter\bin` to environment path variables.

10. Download Java from the official website and install it.

11. Add `JAVA_HOME` as `C:\Program Files\Java\jdk-xx.x` in environment variables.

12. Add `C:\Program Files\Java\jdk-xx.x\bin` to environment path variables.

13. Run the following command to install platforms:  
    ```bash
    sdkmanager platform-tools "platforms;android-30"
    ```

14. Run the following command to create a virtual device:  
    ```bash
    avdmanager create avd -n <DEVICE_NAME> -k "system-images;android-30;google_apis;x86_64"
    ```

15. Run the following command to launch the virtual device:  
    ```bash
    emulator -avd <DEVICE_NAME>
    ```
