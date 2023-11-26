This is a WhatsApp clone app built with Stream Chat SDK to implement messaging systems and Stream Video SDK  using Kotlin and Xml


🛥 Stream Chat & Video SDK
WhatsApp Clone Compose is built with Stream Chat SDK  to implement messaging systems and Stream Video SDK  If you’re interested in adding powerful In-App Messaging to your app, check out the Android Chat Messaging Tutorial!

Stream Chat
Stream Chat SDK for Android on GitHub
Android Samples for Stream Chat SDK on GitHub
Stream Chat Compose UI Components Guidelines
Stream Video
Stream Video SDK for Android on GitHub
Video Call Tutorial
Audio Room Tutorial
Livestream Tutorial
💻 Build Your Own Chat Project
If you want to build your own chat project, you should follow the instructions below:
📷 Previews
 drawing drawing
drawing drawing drawing drawing drawing drawing

🛠 Tech Stack & Open Source Libraries
Minimum SDK level 21.
 Coroutines + Flow for asynchronous.
Chat SDK for Messaging: The Chat Messaging SDK is built on a low-level chat client and provides modular, customizable components that you can easily drop into your app.
Compose Video SDK for Video Calling)

ViewModel: UI related data holder and lifecycle aware.
App Startup: Provides a straightforward, performant way to initialize components at application startup.
Navigation: For navigating screens and Hilt Navigation Compose for injecting dependencies.
Room: Constructs Database by providing an abstraction layer over SQLite to allow fluent database access.
Hilt: Dependency Injection.
Landscapist Glide, animation, placeholder: image loading library that fetches and displays network images with Glide, Coil, and Fresco.
accompanist: A collection of extension libraries for Jetpack Compose
Retrofit2 & OkHttp3: Construct the REST APIs and paging network data.
Retrofit adapters: Retrofit adapters for modeling network responses with Kotlin Result, Jetpack Paging3, and Arrow Either.
ksp: Kotlin Symbol Processing API.
sealedx: Kotlin Symbol Processor to auto-generate extensive sealed classes and interfaces.
StreamLog: A lightweight and extensible logger library for Kotlin and Android.
Baseline Profiles: To improve app performance by including a list of classes and methods specifications in your APK that can be used by Android Runtime.
🏛️ Architecture
WhatsApp Clone Compose follows the Google's official architecture guidance.

architecture

WhatsApp Clone Compose was built with Guide to app architecture, so it would be a great sample to show how the architecture works in real-world projects.

The overall architecture is composed of two layers; UI Layer and the data layer. Each layer has dedicated components and they each have different responsibilities. The arrow means the component has a dependency on the target component following its direction.

Architecture Overview
layer

Each layer has different responsibilities below. Basically, they follow unidirectional event/data flow.

UI Layer
layer

The UI Layer consists of UI elements like buttons, menus, tabs that could interact with users and ViewModel that holds app states and restores data when configuration changes.

Data Layer
layer

The data Layer consists of repositories, which include business logic, such as querying data from the local database and requesting remote data from the network. It is implemented as an offline-first source of business logic and follows the single source of truth principle.

