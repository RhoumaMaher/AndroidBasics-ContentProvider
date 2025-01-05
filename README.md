# Android Basics - Content Providers (Image Access)
This project demonstrates how to access and display images stored in the external storage of an Android device using the `MediaStore` content provider. The app requests the necessary permissions, queries the `MediaStore`, and displays images that were taken within the last 30 days in a scrollable list using Jetpack Compose.

For a detailed explanation of the code and how it works, check out the [Medium article](https://medium.com/@RhoumaMaher/accessing-and-displaying-images-from-external-storage-in-android-using-contentproviders-bd0dbf84b051) on ContentProviders in Android.

## Features
* Request permission to access media images.
* Query the `MediaStore` to retrieve images stored on the device.
* Display images in a scrollable list using `LazyColumn`.
* Use `AsyncImage` from the Coil library for efficient image loading.
* Filter images taken within the last 30 days.
* Display image names along with their respective images.
## Getting Started
### Prerequisites
* Android Studio (latest version recommended).
* A physical Android device or emulator running Android 6.0 (API level 23) or above.
### Clone the Repository
Clone this repository to your local machine.
### Open the Project
1. Open Android Studio.
2. Select **Open an existing Android Studio project.**
3. Navigate to the directory where you cloned the project and select it.
### Permissions
This app requests the `READ_MEDIA_IMAGES` permission to access the images stored on the device's external storage.

On Android 13 and above, the app requests the permission at runtime. For devices running below Android 13, this permission is automatically granted when the app is installed.

### Run the App
1. Connect your device or start an emulator.
2. Click **Run** in Android Studio to install the app on your device or emulator.
3. Once the app is installed, it will query the `MediaStore` and display images that were taken within the last 30 days.
## Project Structure
* **MainActivity.kt:** The main activity of the app where the image access logic is implemented. It includes:
  * Requesting permissions.
  * Querying the MediaStore to get image data.
  * Displaying images using Jetpack Compose.
* **ImageViewModel.kt:** A ViewModel to manage the images and update the UI with the latest data.
* **AndroidManifest.xml:** The manifest file includes the permission for accessing media images
## Libraries Used
* **Jetpack Compose:** A modern Android UI toolkit for building native UI.
* **Coil:** An image loading library for Android, used for asynchronous image loading in `AsyncImage`.
## License
This project is licensed under the MIT License. Feel free to use and modify the code for your own projects. Happy coding! If you have any questions or suggestions, feel free to reach out.
* **Medium:** [My Medium Profile](https://medium.com/@RhoumaMaher)
* **LinkedIn:** [My LinkedIn Profile](https://www.linkedin.com/in/maher-rhouma-581919199/)
  
Let’s connect and discuss all things Android!
