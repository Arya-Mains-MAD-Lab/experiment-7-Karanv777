## Name : Karan Verma
## Roll Number : 23EACAD058
## Experiment Title : GPS Location Application
## Aim : To develop a native application that uses GPS location information.

## Procedure
- Install Flutter SDK
   - Download and install the Flutter SDK from the official website and set up environment variables.
   - Verify installation using:
     ```bash
     flutter doctor
     ```

- Install Android Studio
   - Install Android Studio and configure it with Flutter and Dart plugins.

- Create a New Flutter Project
   - Open Android Studio
   - Click on New Flutter Project
   - Select Flutter Application
   - Enter project name and location
   - Click Finish

- Add Geolocator Dependency
   - Open `pubspec.yaml`
   - Add the following dependency:
     ```yaml
     geolocator: ^latest_version
     ```
   - Run:
     ```bash
     flutter pub get
     ```

- Write the Source Code
   - Open the `main.dart` file and replace the existing code with the given program.
   - The program uses the Geolocator package to:
      - Check if location services are enabled
      - Request location permission
      - Fetch current latitude and longitude using GPS

- Configure Platform Permissions
   - Android:
     Add in `android/app/src/main/AndroidManifest.xml`:
     ```xml
     <uses-permission android:name="android.permission.ACCESS_FINE_LOCATION"/>
     <uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION"/>
     ```

- Connect Device/Emulator
   - Use a physical Android device (recommended for GPS testing) or emulator with location support enabled.

- Run the Application
   - Click Run button or use:
     ```bash
     flutter run
     ```

- Observe the Output
   - On pressing "Get Location" button:
      - App checks GPS service and permissions
      - Displays latitude and longitude of current location

## Output: A Flutter app displaying the current GPS latitude and longitude after pressing the "Get Location" button.

- <img width="1918" height="1028" alt="image" src="https://github.com/user-attachments/assets/f394642e-598c-4ad6-9134-1c2929bb7c21" />


## Conclusion : The experiment was successfully completed by implementing GPS location tracking in Flutter using the Geolocator package and retrieving the device’s current latitude and longitude.
