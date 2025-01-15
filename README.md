Task Manager App
================

app drive link - https://drive.google.com/file/d/1pxmufzXMElKMTshVbdxIJ8ehNr-FdVRH/view?usp=drive_link


screenshot -  [task_manager_ss](https://github.com/user-attachments/assets/ac725126-51a1-4815-a685-3b356a02721f)
-
Setup
-----

### Prerequisites

*   Install Flutter SDK: Flutter Installation Guide
    
*   Android Studio or VS Code for development.
    

### Steps to Run the Project

1.  git clone [https://github.com/your-repo/task-manager-app.gitcd task-manager-app](https://github.com/GAGANRAGHAV/Task_Manager_Flutter.git)
    
2.  flutter pub get
    
3.  flutter run
    
4.  flutter build apk --release The APK will be available in the build/app/outputs/flutter-apk/ directory.
    

Error Handling
--------------

*   **Loading State:** Displays a circular progress indicator while fetching data.
    
*   **Error State:** Shows an error message if the API fails to respond.
    

Challenges Faced
----------------

1.  **API Restriction on HTTP and Internet permission error:**
    
    *   Fixed by enabling android:usesCleartextTraffic="true" in AndroidManifest.xml.
        
2.  **CORS Issues with Local API:**
    
    *   Resolved using a public API or exposing the local API using tools like Ngrok.
        


