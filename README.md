# SearchInCompose
This Android project is a simple example of implementing a search view using Jetpack Compose. The project architecture follows the MVVM (Model-View-ViewModel) pattern with the following components:

View: The UI components that are responsible for displaying the search view and search results to the user. These components are implemented using Jetpack Compose.

ViewModel: The ViewModel is responsible for handling the business logic of the search view. It exposes the search query and search results as LiveData or Flow, which the View can observe and update itself accordingly.

Model: The Model is responsible for handling the data retrieval and manipulation logic of the search view. It communicates with a data source such as a local database or a remote API and returns the search results to the ViewModel.

## Prerequisites
Before setting up this project, make sure you have the following software installed on your machine:
- Android Studio: The latest version of Android Studio can be downloaded from the official website.
- Kotlin: Kotlin is the programming language used to write this project. You can download and install Kotlin from the official website.

## Getting Started
1. To set up this project on Android Studio, follow these steps:
2. Open Android Studio and select "Check out project from Version Control" from the welcome screen.
3. In the "URL" field, enter the URL of the Git repository where this project is hosted. You can either enter the HTTPS or SSH URL.
4. Choose the directory where you want to store the project on your local machine.
5. Click on "Clone" to clone the project from the Git repository.
6. Once the project is cloned, you can open it by selecting "Open an existing Android Studio project" from the welcome screen and selecting the project directory.
7. Android Studio will automatically import the project and set up the necessary dependencies.
8. You can now build and run the project on an emulator or a physical device.


## Architecture overview

The following diagram shows the high-level architecture of the project:

+--------------------------------------+
|                                      |
|                View                  |
|                                      |
+-----------------+--------------------+
|
+-----------------v--------------------+
|                                      |
|              ViewModel               |
|                                      |
+-----------------+--------------------+
|
+-----------------v--------------------+
|                                      |
|                Model                 |
|                                      |
+--------------------------------------+

The View observes the search query and search results from the ViewModel and updates itself accordingly. The ViewModel communicates with the Model to retrieve and manipulate data, and updates the View with the search results.

## Screenshots

![Screenshot_20230215_122016](https://user-images.githubusercontent.com/28220763/218986652-ba8fc85c-aecb-4775-847c-0546f10d88b2.png)



## Library dependencies

This project uses the following libraries:

- Kotlin Coroutines: For handling asynchronous tasks such as data retrieval and manipulation.
- Android Architecture Components: For implementing the MVVM pattern and handling the communication between the View, ViewModel, and Model.
- Jetpack Compose: For implementing the UI components of the search view.
- Kotlin Flows: For exposing the search query and search results as a reactive stream that the View can observe.
- ViewModel: For handling the business logic of the search view and providing the search query and search results to the View.



## License
This project is licensed under the MIT License - see the LICENSE file for details.

