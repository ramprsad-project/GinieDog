To develop an Android application using C# instead of Java/Kotlin, you can use the Xamarin platform. Xamarin allows you to build native Android apps using C# and .NET, making it an excellent choice for C# developers who want to target the Android platform. Here's how you can implement the functionality of collecting data from SQLite DB and sending it to Google Drive using C# and Xamarin:

1. **Android Application (C# with Xamarin)**:
   - Create a new Xamarin.Android project in Visual Studio or Visual Studio for Mac.
   - Set up necessary permissions to access the SQLite database and Google Drive API, just like you would in a Java/Kotlin Android app.
   - Implement code to read data from the SQLite database and create a data dump in a structured format (e.g., JSON) that can be sent to the C# Web API.
   - Use HTTP POST or a suitable method to send the data to the C# Web API. You can use libraries like `HttpClient` to handle HTTP requests in C#.

2. **C# Web API**:
   - Create a new C# Web API project using your preferred framework (e.g., ASP.NET Core).
   - Set up authentication to ensure only authorized requests can access the API (e.g., OAuth or API keys), just like you would in a Java/Kotlin Web API.
   - Implement an API endpoint that receives data from the Android application. This endpoint should handle the data received and save it or process it as needed.
   - Set up the Google Drive API in the Web API project, just like you would in a Java/Kotlin Web API.
   - Implement code to upload the received data dump to Google Drive using the Google Drive API, just like you would in a Java/Kotlin Web API.

3. **Google Drive API**:
   - Create a project on the Google Developers Console and enable the Google Drive API for your project.
   - Set up the necessary credentials (service account or OAuth) to allow the C# Web API to access Google Drive on behalf of the user, just like you would in a Java/Kotlin Web API.

4. **Handling Data in C# Web API**:
   - When the Android application sends data to the Web API, the API endpoint should receive the data and process it accordingly, just like you would in a Java/Kotlin Web API.
   - Parse the data dump received from the Android application and store it in the desired format or database, just like you would in a Java/Kotlin Web API.

5. **Uploading to Google Drive**:
   - Use the Google Drive API client libraries for C# to interact with Google Drive, just like you would in a Java/Kotlin Web API. These libraries provide methods to upload files to Google Drive.
   - After successfully uploading the data dump, you can store the file ID or relevant information in your database for future reference, just like you would in a Java/Kotlin Web API.

6. **Security and Error Handling**:
   - Implement security measures in the Web API to prevent unauthorized access, just like you would in a Java/Kotlin Web API.
   - Handle errors gracefully by providing appropriate error responses to the Android application, just like you would in a Java/Kotlin Web API.

Xamarin.Android allows you to use C# to build the Android application, while the C# Web API can be built using any C# web development framework (e.g., ASP.NET Core). The logic and functionality remain similar to what you would implement in Java/Kotlin for an Android application and Java/Kotlin for a Web API. The main advantage is that you can use your C# skills to develop the entire application stack.