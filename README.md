# Modular Firebase Authentication for Unity

A robust, reusable, and extensible authentication system for Unity projects that integrates with Firebase. It provides a simple, event-driven way to handle multiple sign-in providers.

## Features
- ✅ **Multi-Provider Support:** Handles Google and Anonymous (Guest) sign-in.
- ✅ **Extensible:** Built on an interface-based (`IAuthProvider`) design, making it easy to add new providers.
- ✅ **New User Detection:** Reliably identifies first-time players to trigger profile creation in your database.
- ✅ **Session Persistence:** Automatically signs in returning players for a seamless user experience.
- ✅ **Event-Driven:** Uses C# events to communicate auth status changes to your UI and game systems.
- ✅ **Configurable:** Uses a `ScriptableObject` to manage project-specific keys, keeping them out of the source code.

## Dependencies
- **Firebase Unity SDK** (Authentication)
- **Google Sign-In for Unity** package

## Setup Instructions
1. Import the `.unitypackage`in your Unity project.
2. Follow the setup guides for the Firebase and Google Sign-In SDKs.
3. In your `Assets` window, create a folder named `Resources`.
4. Inside `Resources`, right-click and select **Create > Authentication > Auth Config**.
5. Select the new `AuthConfig` asset and paste your **Google Web Client ID** into the inspector field.
6. Add the `FirebaseInitializer` and `AuthManager` scripts to a persistent GameObject in your first scene.