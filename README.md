# Details

This assignment focuses on web application vulnerabilities and how to fix them. The vulnerable application is written in Java and requires JDK 8 or a newer version installed on your PC. Please install [Java SE Development Kit 11.0.18](https://www.oracle.com/java/technologies/javase/jdk11-archive-downloads.html#:~:text=Java%20SE%20Development%20Kit%2011.0.18). It is compatible with Linux, Mac, and Windows operating systems.

Scenario
You are provided with the source code of a web application in patients.zip Last ned patients.zip. This application represents an initial and rudimentary attempt by an inexperienced developer to build a patient records system. The purpose of the system is to allow General Practitioners (GPs) working in medical practice to log in and search for patient details related to their ongoing treatments.

The application utilises Jetty as an integrated web server. A Java Servlet handles incoming requests. Data storage is implemented using an SQLite 3 database, with queries performed through JDBC. Additionally, HTML pages are dynamically generated using the FreeMarker template engine.

## Analysing Security Vulnerabilities

To execute the web application, navigate to the command line and use the following command:

```bash
./gradlew run
```

If you are using Windows, you can exclude the leading ./ in the command.

To interact with the application, open a web browser and navigate to <http://localhost:8080> . This will allow you to access the application's interface. Utilise the information gathered in Step 1 to navigate through various paths within the application and explore its functionalities.

Examine the application's database to gain access to login credentials and patient details necessary for testing. You can accomplish this task through the command line using the sqlite3 tool. For example, the .schema command will give you a comprehensive database structure overview. Furthermore, you can employ SQL queries directly at the command prompt to thoroughly examine its contents. Alternatively, numerous options are available if you prefer a graphical user interface (GUI). One such example is DB Browser, which offers a user-friendly interface for managing SQLite databases.

## Deliverables

You must submit both your report and the modified application source code. Your report should be in PDF format, limited to 3000 words (excluding any cover sheet and references). The PDF file must be named report.pdf and placed in the same directory as the build.gradle file.

Once you have correctly placed the PDF file in the designated location, execute the following command:

```bash
./gradlew submission
```

This command will generate a file called submission.zip that contains all the necessary materials for submission.

## Submission

Submit the files report.pdf and submission.zip. Although submission.zip already contains the report.pdf file, you must still submit report.pdf as a separate file  on the Canvas submission page. Please note that if report.pdf is not submitted separately as required, your submission will not be accepted.
