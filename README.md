Task Manager App
================

app drive link - https://drive.google.com/file/d/1pxmufzXMElKMTshVbdxIJ8ehNr-FdVRH/view?usp=drive_link

-
screenshot -  [task_manager_ss](https://github.com/user-attachments/assets/ac725126-51a1-4815-a685-3b356a02721f)
-
Setup
-----

### Prerequisites

*   Install Flutter SDK: Flutter Installation Guide
    
*   Android Studio or VS Code for development.
    

### Steps to Run the Project

1.  bashCopy codegit clone https://github.com/your-repo/task-manager-app.gitcd task-manager-app
    
2.  bashCopy codeflutter pub get
    
3.  bashCopy codeflutter run
    
4.  bashCopy codeflutter build apk --releaseThe APK will be available in the build/app/outputs/flutter-apk/ directory.
    

API Integration

---------------

### API Endpoint

*   **URL:** https://jsonplaceholder.typicode.com/todos
    

### Example API Response:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   jsonCopy code[    {      "userId": 1,      "id": 1,      "title": "delectus aut autem",      "completed": false    },    {      "userId": 1,      "id": 2,      "title": "quis ut nam facilis et officia qui",      "completed": true    }  ]   `

### How API Data is Used

*   title: Displayed as the task title.
    
*   completed: Indicates whether the task is completed or not.
    

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
        


