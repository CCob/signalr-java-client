# ASP.NET SignalR for Java 

## Intro

This is is a fork of the original Microsoft SignalR java library.  The root package name has been changed along with a few fixes from fmencias, maks-pasichnyk and others.  I have forked the library for the purpose of having a maven central release along with sources.

Google Gson library has been upgraded to 2.7 along with Java-WebSocket 1.3.7 which is also on central which means no requirments on other repositories 
 
**Note: This library is [NOT compatible](https://github.com/aspnet/SignalR/issues/883#issuecomment-336499189) with ASP.NET Core SignalR 2.0.**

ASP.NET SignalR is a new library for ASP.NET developers that makes it incredibly simple to add real-time web functionality to your applications. What is "real-time web" functionality? It's the ability to have your server-side code push content to the connected clients as it happens, in real-time.

## What can it be used for?
Pushing data from the server to the client (not just browser clients) has always been a tough problem. SignalR makes 
it dead easy and handles all the heavy lifting for you.

This library can be used from both regular Java or Android applications.

## Documentation
See the [documentation](http://asp.net/signalr)
	
## LICENSE
Apache 2.0 License

## Building the source

Clone repo

Open Android Studio, click "Import Non-Android Studio Project" and select the cloned directory 

Build the project.

The signalr-client-sdk.jar will be generated inside the /signalr-client-sdk/build/libs folder

The signalr-client-sdk-android.aar will be generated inside the /signalr-client-sdk-android/build/outputs/aar folder

## Running the tests:
	
Run the signalr-client-tests project as a JUnit test.

## Using the library in a Java application:

Add the signalr-client-sdk.jar and gson library gradle dependencyto the project.

## Using the library in an Android application:

Add the signalr-client-sdk.jar, signalr-client-sdk-android.jar gson library as a gradle dependency to the project.

In the code, before using the library, initialize the platform to use android-specific libraries and compatibility with older Android versions:
	- Platform.loadPlatformComponent(new AndroidPlatformComponent());


## Questions?
The SignalR team hangs out in the [signalr](http://jabbr.net/#/rooms/signalr) room at on [JabbR](http://jabbr.net/).
