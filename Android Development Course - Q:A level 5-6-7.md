# Android Development Course - Q/A level 5-6-7
- - - -

# Level 5 Questions
## 1) 	Explain what the REST architecture is, and explain the role of :

### REST architecture

REST = REPRESENTATIONAL STATE TRANSFER 

* REST = is a collection of network architecture principles which outline how resources are defined and addressed 
* 
The six characteristics of REST: 
1. Uniform interface
2. Decoupled client-server interaction
3. Stateless
4. Cacheable
5. Layered
6. Extensible through code on demand (optional) 

![](Android%20Development%20Course%20-%20Q:A%20level%205-6-7/Screenshot%202018-11-21%20at%2017.27.03.png)

### Resources (represented by URLs)
* The key abstraction of information in REST is a resource (e.g. a piece of text, a movie, a picture). 

### Methods (e.g. GET and POST)
Methods represent the actions to be performed on resources: 

* HTTP GET  - retrieving information
* HTTP POST  - adding new information 
* HTTP PUT -  updating information
* HTTP DELETE - deleting information 

### Representations (e.g. JSON) in this architecture.
* How data is represented or returned to the client for presentation. 
* Two main formats: 
	* JavaScript Object Notation (JSON) 
	* XML 


## 2) 	Explain what a REST backend is.

REST service that’s only used by a single application I’d typically call that a back-end



## 3) 	Give 5 examples of publicly available REST backends that can be accessed by an (Android) app.

[Developers / API | Open Library](https://openlibrary.org/developers/api)

[Calendar API   |  Google Developers](https://developers.google.com/calendar/)

[Blockchain API: Bitcoin API - Blockchain](https://www.blockchain.com/api)

[GitHub API v3 | GitHub Developer Guide](https://developer.github.com/v3/)

[Oxford Dictionaries API](https://developer.oxforddictionaries.com)



## 4) 	What is Firebase?
Firebase is a Backend-as-a-Service — BaaS — that started as a  [YC11 startup](http://blog.ycombinator.com/firebase-yc-s11-raises-5-dollars-dot-6m-series-a-from-union-square-ventures-and-flybridge)  and grew up into a next-generation app-development platform on Google Cloud Platform.
Firebase frees developers to focus crafting fantastic user experiences. You don’t need to manage servers. You don’t need to write APIs. Firebase is your server, your API and your datastore, all written so generically that you can modify it to suit most needs. Yeah, you’ll occasionally need to use other bits of the Google Cloud for your advanced applications. Firebase can’t be everything to everybody. But it gets pretty close.



## 5) 	Elaborate why interfacing with a backend should be a-synchronously (i.e. not on the UI thread) rather than synchronously.


SYNCHRONOUS
You are in a queue to get a movie ticket. You cannot get one until everybody in front of you gets one, and the same applies to the people queued behind you.

ASYNCHRONOUS
You are in a restaurant with many other people. You order your food. Other people can also order their food, they don’t have to wait for your food to be cooked and served to you before they can order. In the kitchen restaurant workers are continuously cooking, serving, and taking orders. People will get their food served as soon as it is cooked.

If someone wants apples compared with apples; if you wanted the restaurant scenario to be synchronous, then when you order food, everyone else in the restaurant would have to wait for your food to arrive before they can order their food etc. Now this seems like a really dumb scenario to be in, but in the computing world this scenario could be useful. Say each customer cant decide what they want, and instead want to look at what the previous customer orders to decide if they want that or not, then it makes sense that they have to wait for the food to arrive before ordering

[Asynchronous vs synchronous execution, what does it really mean? - Stack Overflow](https://stackoverflow.com/questions/748175/asynchronous-vs-synchronous-execution-what-does-it-really-mean)


## 6) 	In level 4 demo we have shown the use of AsyncTask for manipulating an Sql local database. Similarly we can interface with a backend. Once a JSON stream is received from that backend, it is possible to analyse it by decomposition of that JSON stream, using all the keywords and parameters present in that stream. That is a cumbersome process. Explain what the Retrofit and Gson libraries can do for you.
### Retrofit
A type-safe HTTP client for Android and Java
Retrofit is the class through which your API interfaces are turned into callable objects. By default, Retrofit will give you sane defaults for your platform but it allows for customization.

### Gson

Overview
Gson is a Java library that can be used to convert Java Objects into their JSON representation. It can also be used to convert a JSON string to an equivalent Java object. Gson can work with arbitrary Java objects including pre-existing objects that you do not have source code of.

Goals for Gson
* Provide easy to use mechanisms like toString() and constructor (factory method) to convert Java to JSON and vice-versa
* Allow pre-existing unmodifiable objects to be converted to and from JSON
* Allow custom representations for objects
* Support arbitrarily complex objects
* Generate compact and readable JSON output

- - - -

# Level 5 Resources

# REST
 [https://en.wikipedia.org/wiki/Representational_state_transfer](https://www.google.com/url?q=https://en.wikipedia.org/wiki/Representational_state_transfer&sa=D&ust=1543949020159000) 

 [https://stackoverflow.com/questions/671118/what-exactly-is-restful-programming](https://www.google.com/url?q=https://stackoverflow.com/questions/671118/what-exactly-is-restful-programming&sa=D&ust=1543949020160000) 

 [https://freshinup.com/build-apps-with-api-backend/](https://www.google.com/url?q=https://freshinup.com/build-apps-with-api-backend/&sa=D&ust=1543949020161000) 

 [https://firebase.google.com](https://www.google.com/url?q=https://firebase.google.com&sa=D&ust=1543949020162000) 

# Retrofit, GSON
 [https://square.github.io/retrofit/](https://www.google.com/url?q=https://square.github.io/retrofit/&sa=D&ust=1543949020163000) 

 [https://github.com/codepath/android_guides/wiki/Consuming-APIs-with-Retrofit](https://www.google.com/url?q=https://github.com/codepath/android_guides/wiki/Consuming-APIs-with-Retrofit&sa=D&ust=1543949020164000) 

 [https://guides.codepath.com/android/consuming-apis-with-retrofit](https://www.google.com/url?q=https://guides.codepath.com/android/consuming-apis-with-retrofit&sa=D&ust=1543949020165000) 

 [http://www.vogella.com/tutorials/Retrofit/article.html](https://www.google.com/url?q=http://www.vogella.com/tutorials/Retrofit/article.html&sa=D&ust=1543949020165000) 

 [http://mobilesiri.com/retrofit-tutorial-android-studio/](https://www.google.com/url?q=http://mobilesiri.com/retrofit-tutorial-android-studio/&sa=D&ust=1543949020166000) 

 [https://www.androidhive.info/2016/05/android-working-with-retrofit-http-library/](https://www.google.com/url?q=https://www.androidhive.info/2016/05/android-working-with-retrofit-http-library/&sa=D&ust=1543949020166000) 

 [https://github.com/google/gson/blob/master/UserGuide.md](https://www.google.com/url?q=https://github.com/google/gson/blob/master/UserGuide.md&sa=D&ust=1543949020167000) 


- - - -

# Level 6 Questions
[Fragment Navigation Pattern in Android | Toptal](https://www.toptal.com/android/android-fragment-navigation-pattern)
## 1 	Why don’t you need to declare a fragment inside your Manifest?
Cleaner and more maintainable AndroidManifest.xml*
Now that we have only one Activity, we no longer need to update the manifest every time we add a new screen. Unlike activities, we do not have to declare fragments.
This could seem like a minor thing, but for larger applications which have 50+ activities this can significantly improve readability of the AndroidManifest.xml file.


## 2 	What Java class needs to be extended, in order to create a fragment?
To create a fragment, extend the  [Fragment](https://developer.android.com/reference/android/support/v4/app/Fragment.html)  class, then override key lifecycle methods to insert your app logic, similar to the way you would with an  [Activity](https://developer.android.com/reference/android/app/Activity.html)  class.
One difference when creating a  [Fragment](https://developer.android.com/reference/android/support/v4/app/Fragment.html)  is that you must use the  [onCreateView()](https://developer.android.com/reference/android/support/v4/app/Fragment.html#onCreateView(android.view.LayoutInflater,%20android.view.ViewGroup,%20android.os.Bundle))  callback to define the layout. In fact, this is the only callback you need in order to get a fragment running.

## 3 	How do you communicate from one fragment to another fragment?
In order to reuse the Fragment UI components, you should build each as a completely self-contained, modular component that defines its own layout and behavior. Once you have defined these reusable Fragments, you can associate them with an Activity and connect them with the application logic to realize the overall composite UI.
Often you will want one Fragment to communicate with another, for example to change the content based on a user event. All Fragment-to-Fragment communication is done either through a shared  [ViewModel](https://developer.android.com/reference/android/arch/lifecycle/ViewModel)  or through the associated Activity. Two Fragments should never communicate directly.
The recommended way to communicate between fragments is to create a shared  [ViewModel](https://developer.android.com/reference/android/arch/lifecycle/ViewModel)  object. Both fragments can access the ViewModel through their containing Activity. The Fragments can update data within the ViewModel and if the data is exposed using  [LiveData](https://developer.android.com/reference/android/arch/lifecycle/LiveData)  the new state will be pushed to the other fragment as long as it is observing the LiveData from the ViewModel. To see how to implement this kind of communication, read the ‘Share data between Fragments’ section in the  [ViewModel guide](https://developer.android.com/topic/libraries/architecture/viewmodel.html) .
If you are unable to use a shared ViewModel to communicate between your Fragments you can manually implement a communication flow using interfaces. However this ends up being more work to implement and it is not easily reusable in other Fragments.


## 4 	In the lifecycle of a fragment, what method is called as soon as the view is visible?
 [onCreateView()](https://developer.android.com/reference/android/support/v4/app/Fragment.html#onCreateView(android.view.LayoutInflater,%20android.view.ViewGroup,%20android.os.Bundle)) The system calls this when it’s time for the fragment to draw its user interface for the first time. To draw a UI for your fragment, you must return a  [View](https://developer.android.com/reference/android/view/View.html)  from this method that is the root of your fragment’s layout. You can return null if the fragment does not provide a UI.

## 5 	Is it possible to access a fragment, even if the lifecycle of its host activity has ended? Explain why.
[1.2: Fragment lifecycle and communications · GitBook](https://google-developer-training.github.io/android-developer-advanced-course-concepts/unit-1-expand-the-user-experience/lesson-1-fragments/1-2-c-fragment-lifecycle-and-communications/1-2-c-fragment-lifecycle-and-communications.html)



## 6 	A record of all Fragment transactions is kept for each Activity by the FragmentManager. Why can this be useful?

When designing your application to support a wide range of screen sizes, you can reuse your fragments in different layout configurations to optimize the user experience based on the available screen space.
For example, on a handset device it might be appropriate to display just one fragment at a time for a single-pane user interface. Conversely, you may want to set fragments side-by-side on a tablet which has a wider screen size to display more information to the user.
![](Android%20Development%20Course%20-%20Q:A%20level%205-6-7/fragments-screen-mock.png)
**Figure 1.** Two fragments, displayed in different configurations for the same activity on different screen sizes. On a large screen, both fragments fit side by side, but on a handset device, only one fragment fits at a time so the fragments must replace each other as the user navigates.
The  [FragmentManager](https://developer.android.com/reference/android/support/v4/app/FragmentManager.html)  class provides methods that allow you to add, remove, and replace fragments to an activity at runtime in order to create a dynamic experience.

- - - -
## Level 6  Resources

 [https://developer.android.com/guide/components/fragments](https://www.google.com/url?q=https://developer.android.com/guide/components/fragments&sa=D&ust=1541773979069000) 

 [https://github.com/codepath/android_guides/wiki/Creating-and-Using-Fragments](https://www.google.com/url?q=https://github.com/codepath/android_guides/wiki/Creating-and-Using-Fragments&sa=D&ust=1541773979069000) 

- - - -

# Level 7 Resources
## 1 	What are the four parts that Android Architecture Components consist of?
[Android Architecture Components – ProAndroidDev](https://proandroiddev.com/android-architecture-components-cb1ea88d3835)

![](Android%20Development%20Course%20-%20Q:A%20level%205-6-7/1*kEjRZjzQ4lxgMITbU8iidg.png)

Android architecture components are a collection of libraries that help you design robust, testable, and maintainable apps. Start with classes for managing your UI component lifecycle and handling data persistence.

1. Manage your app’s lifecycle with ease. New  [lifecycle-aware components](https://developer.android.com/topic/libraries/architecture/lifecycle)  help you manage your activity and fragment lifecycles. Survive configuration changes, avoid memory leaks and easily load data into your UI.
2. Use  [LiveData](https://developer.android.com/topic/libraries/architecture/livedata)  to build data objects that notify views when the underlying database changes.
3.  [ViewModel](https://developer.android.com/topic/libraries/architecture/viewmodel)  Stores UI-related data that isn’t destroyed on app rotations.
4. [Room](https://developer.android.com/topic/libraries/architecture/room)  is an a SQLite object mapping library. Use it to Avoid boilerplate code and easily convert SQLite table data to Java objects. Room provides compile time checks of SQLite statements and can return RxJava, Flowable and LiveData observables.

## 2 	Can you name three advantages of using LiveData?
Using LiveData provides the following advantages:
**Ensures your UI matches your data state**
LiveData follows the observer pattern. LiveData notifies  [Observer](https://developer.android.com/reference/android/arch/lifecycle/Observer.html)  objects when the lifecycle state changes. You can consolidate your code to update the UI in these Observer objects. Instead of updating the UI every time the app data changes, your observer can update the UI every time there’s a change.
**No memory leaks**
Observers are bound to  [Lifecycle](https://developer.android.com/reference/android/arch/lifecycle/Lifecycle.html)  objects and clean up after themselves when their associated lifecycle is destroyed.
**No crashes due to stopped activities**
If the observer’s lifecycle is inactive, such as in the case of an activity in the back stack, then it doesn’t receive any LiveData events.
**No more manual lifecycle handling**
UI components just observe relevant data and don’t stop or resume observation. LiveData automatically manages all of this since it’s aware of the relevant lifecycle status changes while observing.
**Always up to date data**
If a lifecycle becomes inactive, it receives the latest data upon becoming active again. For example, an activity that was in the background receives the latest data right after it returns to the foreground.
**Proper configuration changes**
If an activity or fragment is recreated due to a configuration change, like device rotation, it immediately receives the latest available data.
**Sharing resources**
You can extend a  [LiveData](https://developer.android.com/reference/android/arch/lifecycle/LiveData.html)  object using the singleton pattern to wrap system services so that they can be shared in your app. The LiveData object connects to the system service once, and then any observer that needs the resource can just watch the LiveData object. For more information, see Extend LiveData.


## 3 	What is the purpose of a ViewModel?
The  [ViewModel](https://developer.android.com/reference/android/arch/lifecycle/ViewModel.html)  class is designed to store and manage UI-related data in a lifecycle conscious way. The  [ViewModel](https://developer.android.com/reference/android/arch/lifecycle/ViewModel.html)  class allows data to survive configuration changes such as screen rotations.


## 4 	What are the three major components of ROOM?
There are 3 major components in Room:
*  [Database:](https://developer.android.com/reference/androidx/room/Database.html)  Contains the database holder and serves as the main access point for the underlying connection to your app’s persisted, relational data.
The class that’s annotated with  [@Database](https://developer.android.com/reference/androidx/room/Database.html)  should satisfy the following conditions:
	* Be an abstract class that extends  [RoomDatabase](https://developer.android.com/reference/androidx/room/RoomDatabase.html) .
	* Include the list of entities associated with the database within the annotation.
	* Contain an abstract method that has 0 arguments and returns the class that is annotated with  [@Dao](https://developer.android.com/reference/androidx/room/Dao.html) .
* At runtime, you can acquire an instance of  [Database](https://developer.android.com/reference/androidx/room/Database.html)  by calling   Room.databaseBuilder() or Room.inMemoryDatabaseBuilder()
*  [Entity:](https://developer.android.com/training/data-storage/room/defining-data.html)  Represents a table within the database.
*  [DAO:](https://developer.android.com/training/data-storage/room/accessing-data.html)  Contains the methods used for accessing the database.


## 5 	Whats the name of the layer often put between the database layer and the viewmodel?
[Applying Google’s Android architecture with ObjectBox database](https://proandroiddev.com/applying-googles-android-architecture-with-objectbox-database-5153ce8ffac1)
The repository is responsible for passing requests from the ViewModel to the database and the network, and returning the response.

- - - -

## Level 7 - Resources

## Android Architecture Components
 [https://developer.android.com/topic/libraries/architecture/](https://www.google.com/url?q=https://developer.android.com/topic/libraries/architecture/&sa=D&ust=1543948860250000) 
https://developer.android.com/jetpack/docs/guide
 
LiveData
 [https://developer.android.com/topic/libraries/architecture/livedata](https://www.google.com/url?q=https://developer.android.com/topic/libraries/architecture/livedata&sa=D&ust=1543948860251000) 
 
ViewModel
 [https://developer.android.com/topic/libraries/architecture/viewmodel](https://www.google.com/url?q=https://developer.android.com/topic/libraries/architecture/viewmodel&sa=D&ust=1543948860252000) 
 
Room
https://developer.android.com/training/data-storage/room/

- - - -

