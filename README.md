GithubPackages for ONLYOFFICE Documents for Android
==================================

This repo contains the GithubPackages for the ONLYOFFICE Documents app for Android (based on binary codes) and describes how the dependencies are used for the app building process.

GithubPackages is a convenient way for creating a modular app architecture and reusing/distributing code across apps or with other developers.

ONLYOFFICE Documents app for Android is a complete mobile office suite. It allows users to work with all types of office files, including docs, sheets, slides, and forms. You are able to create, edit, save and export documents, collaborate on them in real time, fill out forms, view PDFs and  images.

## Components

ONLYOFFICE editors for Android contain the following components:

* __x2t__ is used to enable conversion between the most popular office file formats (DOC, DOCX, ODT, RTF, TXT, PDF, HTML, EPUB, XPS, DjVu, XLS, XLSX, ODS, CSV, PPT, PPTX, ODP). This component is required for proper work of the editors.
* __editors__, __geditors__ basis for editors.
* __docs__, __gdocs__ is used to view and edit text documents, open and fill out OFORM forms.
* __cells__, __gcells__ is used to view and edit spreadsheets.
* __slides__, __gslides__ is used to view and edit presentations.

## How Use

* Main project [ONLYOFFICE Documents](https://github.com/ONLYOFFICE/documents-app-android)

* Add the following code to build.gradle inside the app module that will be using the library published on GitHub Packages

```
maven {
  name = "GitHubPackages"
  url = uri("https://maven.pkg.github.com/$userId/$repository")
} 
```
* Inside dependencies of the build.gradle of app module, use the following code

```
dependencies {
  implementation("com.onlyoffice.android:$artifactId:$version') 
}
```
## Project Information

Official website: [www.onlyoffice.com](https://www.onlyoffice.com/)

Project page: [www.onlyoffice.com/office-for-android.aspx](https://www.onlyoffice.com/office-for-android.aspx)

## User Feedback and Support

If you face any problems or have questions about ONLYOFFICE app for Android, please visit our official forum at [forum.onlyoffice.com][1]. You can also refer to [Stack Overflow][2].

[1]: https://forum.onlyoffice.com/c/mobile-apps/36
[2]: http://stackoverflow.com/questions/tagged/onlyoffice
