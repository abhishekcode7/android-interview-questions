### MIXED QUESTIONS

- **Question**: What is an inline function in Kotlin?
    - **Answer**: replaced with function code during compile time
- **Question**: What is the advantage of using const in Kotlin?
    - **Answer**: replaced with value at compile time and prevents variable call overhead
- **Question**: What is a reified keyword in Kotlin?
    - **Answer**: used to preserve generic type , ex: inline fun <reified T> Gson.fromJson().
- **Question**: Suspending vs Blocking in Kotlin Coroutines
    - **Answer**: sus does not block thread while Blocking does block thread.
- **Question**: Launch vs Async in Kotlin Coroutines
    - **Answer**: launch does not return anything but asnc returns result.
- **Question**: internal visibility modifier in Kotlin
    - **Answer**: class only available inside module.
- **Question**: open keyword in Kotlin
    - **Answer**: OPEN for inheritance , classes are final by default.
- **Question**: lateinit vs lazy in Kotlin
    - **Answer**: done.
- **Question**: What is Multidex in Android?
    - **Answer**: done
- **Question**: How does the Android Push Notification system work?
    - **Answer**: done
- **Question**: How does the Kotlin Multiplatform work?
    - **Answer**: [How does the Kotlin Multiplatform work?](https://www.youtube.com/watch?v=nwfNh6Kd5hI)
- **Question**: What is a ViewModel and how is it useful?
    - **Answer**: Viewmodel persists data in lifecycle conscious way.
- **Question**: Is it possible to force the Garbage Collection in Android?
    - **Answer**: No, we can request by calling gc.collect() , but cannot force.
- **Question**: What is a JvmStatic Annotation in Kotlin?
    - **Answer**: tells compiler to create a static implementation of method which can be called by java.
- **Question**: init block in Kotlin
    - **Answer**: runs after primary constructor nd before secondary , used to initialise variables.
- **Question**: JvmField Annotation in Kotlin
    - **Answer**: exposes variables as field and no need to call getters, setters.
- **Question**: singleTask launchMode in Android
    - **Answer**: done
- **Question**: Difference between == and === in Kotlin
    - **Answer**: done
- **Question**: JvmOverloads Annotation in Kotlin
    - **Answer**: done
- **Question**: Why is it recommended to use only the default constructor to create a Fragment?
    - **Answer**: done
- **Question**: Why do we need to call setContentView() in onCreate() of Activity class?
    - **Answer**: done
- **Question**: When only onDestroy is called for an activity without onPause() and onStop()?
    - **Answer**: when onDestroy called in onCreate.

### Kotlin Coroutines

Topics you should know in **Kotlin Coroutines** for Android Interview:

* coroutines
* suspend
* launch, async-await, withContext
* dispatchers
* scope, context, job
* lifecycleScope, viewModelScope, GlobalScope
* suspendCoroutine, suspendCancellableCoroutine
* coroutineScope, supervisorScope

### Kotlin Flow API

Topics you should know in **Kotlin Flow API** for Android Interview:

* Flow Builder, Operator, Collector
* flowOn, dispatchers
* Operators such as filter, map, zip, flatMapConcat, retry, debounce, distinctUntilChanged, flatMapLatest
* Terminal operators
* Cold Flow vs Hot Flow
* StateFlow, SharedFlow, callbackFlow, channelFlow

### Kotlin

Android Interview Questions and Answers:

* **What are `companion objects` in Kotlin?** - Static values are stored in them.

* **Extension functions** - ✅

* **What is a data class in Kotlin?** - ✅

* **noinline in Kotlin** - [Learn from here](https://outcomeschool.com/blog/noinline-in-kotlin)

* **crossinline in Kotlin** - [Learn from here](https://outcomeschool.com/blog/crossinline-in-kotlin)

* **scope functions in Kotlin** - let,run,with,apply,also

* **What are higher-order functions in Kotlin?** - ✅

* **Write a function(Higher-Order Function) that returns a function.** - [Check solution here](https://x.com/amitiitbhu/status/1862721662208155800)

* **What are Lambdas in Kotlin** - ✅

* **What is runBlocking in Coroutines?** - ✅

* **What is the meaning of structured concurrency in Kotlin Coroutines?** - [Learn from here](https://www.linkedin.com/posts/outcomeschool_softwareengineer-androiddev-android-activity-7267476661967683584-wDCh/)

* **What is the difference between `val` and `var`?** - ✅

* **How to check if a `lateinit` variable has been initialized?** - variable.isInitialized() ✅

* **How to do lazy initialization of variables in Kotlin?** - ✅

* **What are the visibility modifiers in Kotlin?** - [Learn from here](https://kotlinlang.org/docs/visibility-modifiers.html)

* **What is the equivalent of Java static methods in Kotlin?** - companion object

* **How to create a Singleton class in Kotlin?** - object:

* **What is the difference between `open` and `public` in Kotlin?** - [Learn from here](https://outcomeschool.com/blog/open-keyword-in-kotlin)

* **Explain the use-case of `let`, `run`, `with`, `also`, `apply` in Kotlin.** - ✅

* **How to choose between `apply` and `with`?** -  ✅

* **What are `Labels` in Kotlin?** - [Learn from here](https://kotlinlang.org/docs/returns.html)

* **What are Coroutines in Kotlin?** - ✅

* **What is Coroutine Scope?** - ✅

* **Scopes in Kotlin Coroutines Used in Android** - ✅

* **What is Coroutine Context?** - ✅

* **Launch vs Async in Kotlin Coroutines** - ✅

* **Thread.sleep() vs delay() in Kotlin** - ✅

* **When to use Kotlin sealed classes?** - when we have states of similar type of data ,better customization than Enums ✅

* **Tell about the Collections in Kotlin** - [Learn from here](https://kotlinlang.org/docs/collections-overview.html)

* **What does ?: do in Kotlin? (Elvis Operator)** - ✅

* **timeouts in Kotlin Coroutines** - [Learn from here](https://www.linkedin.com/posts/outcomeschool_softwareengineer-androiddev-android-activity-7265684677770846208-Ug0Y)

* **How do you combine multiple coroutine results?** - [Learn from here](https://www.linkedin.com/posts/outcomeschool_softwareengineer-androiddev-android-activity-7267827335393873920-v6t3)

* **What is a Job in Coroutines?** - ✅

* **How to Implement Debounce Using Coroutines?** - [Learn from here](https://www.linkedin.com/posts/amit-shekhar-iitbhu_softwareengineer-androiddev-android-activity-7285163906686164994-tOUK)

### Android

Android Interview Questions and Answers:

#### Base

* **Why does an Android App lag?** - gc runs frequently,image loading libraries not used in RV ✅

* **What is `Context`? How is it used?** - ✅

* **Tell all the Android application components.** - Activities, Services, Broadcast Receivers, Content providers ✅

* **What is `AndroidManifest.xml`?** - ✅

* **What is the `Application` class?**
    - The Application class in Android is the base class within an Android app that contains all other components such as activities and services. The Application class, or any subclass of the Application class, is instantiated before any other class when the process for your application/package is created.

#### Activity and Fragment

* **What is `Activity` and its lifecycle?** - ✅

* **What is the difference between onCreate() and onStart()** - onCreate view is initialized , onStart view is made visible ✅

* **What is onSaveInstanceState() and onRestoreInstanceState() in activity?**
    - onSaveInstanceState() - This method is used to store data before pausing the activity.
    - onRestoreInstanceState() - This method is used to recover the saved state of an activity when the activity is recreated after destruction. So, the onRestoreInstanceState() receives the bundle that contains the instance state information.

* **What is `Fragment` and its lifecycle?** - [Learn from here](https://developer.android.com/guide/fragments/lifecycle)

* **What are "launchMode"?** - standard, singleTop, singleTask, SingleInstance. ✅

* **What is the difference between a `Fragment` and an `Activity`? Explain the relationship between the two.** - [Learn from here](https://stackoverflow.com/questions/10478233/why-fragments-and-when-to-use-fragments-instead-of-activities)

* **When should you use a Fragment rather than an Activity?**
    - When you have some UI components to be used across various activities
    - When multiple views can be displayed side by side just like ViewPager

* **What is the difference between adding/replacing fragment in backstack?** - [Learn from here](https://stackoverflow.com/questions/24466302/basic-difference-between-add-and-replace-method-of-fragment/24466345)

* **How would you communicate between two Fragments?** - interface , shared viewmodel ✅

* **What is retained `Fragment`?** - [Learn from here](https://www.linkedin.com/posts/outcomeschool_softwareengineer-androiddev-android-activity-7265620144289193984-hlpH)

* **What is the purpose of `addToBackStack()` while commiting fragment transaction?**
    - By calling addToBackStack(), the replace transaction is saved to the back stack so the user can reverse the transaction and bring back the previous fragment by pressing the Back button. For more [Learn from here](https://stackoverflow.com/questions/22984950/what-is-the-meaning-of-addtobackstack-with-null-parameter)

#### Views and ViewGroups

* **Optimizing layouts in Android** - [Learn from here](https://www.linkedin.com/posts/amit-shekhar-iitbhu_softwareengineer-androiddev-android-activity-7269208182390951936-dAg3)

* **What is `View` in Android?** - Rectangular area on screen with which user can interact ✅

* **Difference between `View.GONE` and `View.INVISIBLE`?** - [Learn from here](https://stackoverflow.com/questions/11556607/android-difference-between-invisible-and-gone)

* **Can you a create custom view? How?** - Yes, programatically. ✅

* **What are ViewGroups and how they are different from the Views?**
    - View: View objects are the basic building blocks of User Interface(UI) elements in Android. View is a simple rectangle box which responds to the user’s actions. Examples are EditText, Button, CheckBox etc. View refers to the android.view.View class, which is the base class of all UI classes.
    - ViewGroup: ViewGroup is the invisible container. It holds View and ViewGroup. For example, LinearLayout is the ViewGroup that contains Button(View), and other Layouts also. ViewGroup is the base class for Layouts.

* **What is a Canvas?**

* **What is a `SurfaceView`?** - [Learn from here](https://developer.android.com/reference/android/view/SurfaceView)

* **Relative Layout vs Linear Layout.**

* **Tell about Constraint Layout** ✅

* **Do you know what is the view tree? How can you optimize its depth?** - [Learn from here](https://developer.android.com/reference/android/view/ViewTreeObserver)

#### Displaying Lists of Content

* **What is the difference between `ListView` and `RecyclerView`?** - RV enforces Viewholder , ListView only allows vertical scrolling , RV has item animations ✅

* **How does the RecyclerView work?** - ✅

* **RecyclerView Optimization - Scrolling Performance Improvement** - [Learn from here](https://outcomeschool.com/blog/recyclerview-optimization)

* **Optimizing Nested RecyclerView** - [Learn from here](https://outcomeschool.com/blog/setrecycledviewpool-for-optimizing-nested-recyclerview)

* **How does RecyclerView improve performance over ListView?** - ✅

* **What are the components of a RecyclerView?**

* **Explain the role of RecyclerView.Adapter and RecyclerView.ViewHolder** - ✅

* **What is a LayoutManager in RecyclerView?**

* **How do you handle multiple view types in a single RecyclerView?** - give id to each view ✅

* **What is DiffUtil and how does it improve RecyclerView performance?** - [Learn from here](https://www.linkedin.com/posts/amit-shekhar-iitbhu_softwareengineer-androiddev-android-activity-7279435764973686785-pfiQ)

* **What is the purpose of RecyclerView.setHasFixedSize(true)?** - [Learn from here](https://www.linkedin.com/posts/amit-shekhar-iitbhu_softwareengineer-androiddev-android-activity-7282252857637007361-thzv/)

* **How do you update a specific item in RecyclerView?** - notifyItemChanged(index) ✅

* **What is `SnapHelper`?** - Learn from here: [SnapHelper](https://outcomeschool.com/blog/snaphelper)

#### Dialogs and Toasts

* **What is `Dialog` in Android?** - ✅

* **What is `Toast` in Android?** - ✅

* **What the difference between `Dialog` and `Dialog Fragment`?** - [Learn from here](https://stackoverflow.com/questions/7977392/android-dialogfragment-vs-dialog)

#### Intents and Broadcasting

* **What is `Intent`?** - action we want to perform ✅

* **What is an Implicit `Intent`?** - ✅
        
* **What is an Explicit `Intent`?** - ✅

* **What is a `BroadcastReceiver`?** - ✅

* **What is a Sticky `Intent`?**
    - Sticky Intents allows communication between a function and a service. sendStickyBroadcast() performs a sendBroadcast(Intent) known as sticky, i.e. the Intent you are sending stays around after the broadcast is complete, so that others can quickly retrieve that data through the return value of registerReceiver(BroadcastReceiver, IntentFilter). For example, if you take an intent for ACTION_BATTERY_CHANGED to get battery change events: When you call registerReceiver() for that action — even with a null BroadcastReceiver — you get the Intent that was last Broadcast for that action. Hence, you can use this to find the state of the battery without necessarily registering for all future state changes in the battery.

* **Describe how broadcasts and intents work to be able to pass messages around your app?** - [Learn from here](https://stackoverflow.com/questions/7276537/using-a-broadcast-intent-broadcast-receiver-to-send-messages-from-a-service-to-a)

* **What is a `PendingIntent`?**
    - If you want someone to perform any Intent operation at future point of time on behalf of you, then we will use Pending Intent.

* **What are the different types of Broadcasts?** - [Learn from here](https://developer.android.com/guide/components/broadcasts)

#### Services

* **Explain Android Service Lifecycle** - [Learn from here](https://www.linkedin.com/posts/amit-shekhar-iitbhu_softwareengineer-androiddev-android-activity-7265212180570992640-CJn_)

* **What is Service?** - [Learn from here](https://developer.android.com/guide/components/services)

* **On which thread does a Service run in Android?** - main by default ✅

* **Service vs IntentService** - [Learn from here](https://stackoverflow.com/questions/15524280/service-vs-intentservice-in-the-android-platform)

* **What is a Foreground Service?** - [Learn from here](https://developer.android.com/develop/background-work/services/foreground-services)

* **What is a `JobScheduler`?** - [Learn from here](https://developer.android.com/reference/android/app/job/JobScheduler)

#### Inter-process Communication

* **How can two distinct Android apps interact?** - intents, broadcasts, sharedpreferences , contentproviders.

* **Is it possible to run an Android app in multiple processes? How?** - [Learn from here](https://stackoverflow.com/questions/6567768/how-can-an-android-application-have-more-than-one-process)

* **What is AIDL? Enumerate the steps in creating a bounded service through AIDL.** - [Learn from here](https://developer.android.com/guide/components/aidl)

* **What can you use for background processing in Android?** - coroutines,services,workmanager ✅

* **What is a `ContentProvider` and what is it typically used for?** - [Learn from here](https://www.linkedin.com/posts/outcomeschool_softwareengineer-androiddev-android-activity-7268117553040764931-64fI)

#### Long-running Operations

* **How to run parallel tasks and get a callback when all are complete?** - [Long-running tasks in parallel with Kotlin Flow](https://outcomeschool.com/blog/long-running-tasks-in-parallel-with-kotlin-flow)

* **What is ANR? How can the ANR be prevented?** - [Learn from here](https://developer.android.com/topic/performance/vitals/anr.html)

* **What is an `AsyncTask`(Deprecated in API level 30) ?**

* **What are the problems in AsyncTask?**

* **Daemon Threads vs. User Threads** - [Learn from here](https://x.com/amitiitbhu/status/1817783254885478872)

* **Explain `Looper`, `Handler`, and `HandlerThread`.**

* **Android Memory Leak and Garbage Collection** ✅

* **Can you explain the difference between a Runnable and a Thread in Android?** - [Learn from here](https://www.linkedin.com/posts/outcomeschool_softwareengineer-androiddev-android-activity-7279784055284420609-Xa8b)

#### Working With Multimedia Content

* **How do you handle bitmaps in Android as it takes too much memory?** - [Learn from here](https://developer.android.com/topic/performance/graphics/load-bitmap) and [here](https://developer.android.com/topic/performance/graphics/manage-memory)

* **Tell about the `Bitmap` pool.** - [Learn from here](https://outcomeschool.com/blog/bitmap-pool)

#### Data Saving

* **Jetpack DataStore Preferences** - [Learn from here](https://outcomeschool.com/blog/jetpack-datastore-preferences)

* **How to persist data in an Android app?**

* **What is ORM? How does it work?**

* **How would you preserve the `Activity` state during a screen rotation?** - ✅

* **What are different ways to store data in your Android app?** - preference , internal storage, database, server. ✅

* **Explain Scoped Storage in Android.**

* **How to encrypt data in Android?**

* **What is commit() and apply() in SharedPreferences?**
    - commit() returns a boolean value of success or failure immediately by writing data synchronously.
    - apply() is asynchronous and it won't return any boolean response. If you have an apply() outstanding and you are performing commit(), then the commit() will be blocked until the apply() is not completed.

#### Look and Feel

* **What is a `Spannable`?**

* **What is a `SpannableString`?**
   - A SpannableString has immutable text, but its span information is mutable. Use a SpannableString when your text doesn't need to be changed but the styling does. Spans are ranges over the text that include styling information like color, heighliting, italics, links, etc

* **What are the best practices for using text in Android?**

* **How to implement Dark mode in any application?** - Theme ✅

#### Memory Optimizations

* **What is the `onTrimMemory()` method?** - called when system has low memory and we can clean up space ✅

* **How to identify and fix OutOfMemory issues?**

* **How do you find memory leaks in Android applications?**

#### Battery Life Optimizations

* **How to reduce battery usage in an android application?**

* **What is `overdraw`?** - [Learn from here](https://developer.android.com/topic/performance/rendering/overdraw.html)

#### Supporting Different Screen Sizes

* **How do you support different types of resolutions?** - [Learn from here](https://developer.android.com/training/multiscreen/screensizes)

#### Permissions

* **What are the different protection levels in permission?**

#### Native Programming

* **What is the NDK and why is it useful?** - Learn from here: [Android NDK and RenderScript](https://outcomeschool.com/blog/ndk-and-renderscript)

* **What is renderscript?** - Learn from here: [Android NDK and RenderScript](https://outcomeschool.com/blog/ndk-and-renderscript)

#### Android System Internal

* **What is Android Runtime?** - [Android Runtime](https://outcomeschool.com/blog/dalvik-art-jit-aot)

* **Dalvik, ART, JIT, and AOT in Android** - [Dalvik, ART, JIT, and AOT](https://outcomeschool.com/blog/dalvik-art-jit-aot)

* **What are the differences between Dalvik and ART?** - [Difference between Dalvik and ART](https://outcomeschool.com/blog/dalvik-art-jit-aot)

* **What is DEX?** - [Learn from here](https://developer.android.com/reference/dalvik/system/DexFile)

* **What is Multidex in Android?** - [Learn from here](https://www.youtube.com/watch?v=R0zd8lmHnmE)

#### Android Jetpack

* **What is Android Jetpack and why to use this?**

* **What are Android Architecture Components?**

* **What is LiveData in Android?** - ✅

* **How LiveData is different from ObservableField?**

* **What is the difference between setValue and postValue in LiveData?** Learn: [setValue() vs postValue() in LiveData](https://www.linkedin.com/posts/outcomeschool_softwareengineer-androiddev-android-activity-7274283452563107840-SXXl)

* **Explain WorkManager and its use cases.** - ✅

* **How does ViewModel work internally?**

#### Others

* **What is the difference between Serializable and Parcelable? Which is the best approach in Android?** - ✅

* **Why Bundle class is used for data passing and why cannot we use simple Map data structure?** - ✅

* **How do you troubleshoot a crashing application?** - ✅

* **What is AAPT?** - [Learn from here](https://developer.android.com/studio/command-line/aapt2)

* **FlatBuffers vs JSON.**

* **What are Annotations?** - [Learn from here](https://outcomeschool.com/blog/creating-custom-annotations)

* **How to create custom Annotation?** - [Learn from here](https://outcomeschool.com/blog/creating-custom-annotations)

* **What is the Android Support Library? Why was it introduced?** - [Learn from here](https://www.linkedin.com/posts/outcomeschool_androiddev-activity-7275725268680392705-waUi)

* **What is Android Data Binding?**

### Android Libraries

Android Interview Questions and Answers:

* **Explain OkHttp Interceptor** - [Learn from here](https://outcomeschool.com/blog/okhttp-interceptor)

* **OkHttp - HTTP Caching** - [Learn from here](https://outcomeschool.com/blog/caching-with-okhttp-interceptor-and-retrofit)

* **How to enable logging in OkHttp?** - [Learn from here](https://www.linkedin.com/posts/outcomeschool_softwareengineer-androiddev-android-activity-7274652524433850368-qC4D)

* **Why do we use the Dependency Injection Framework like Dagger in Android?** - [Learn from here](https://www.linkedin.com/posts/amit-shekhar-iitbhu_androiddev-activity-7038019147737276417-tH4s)

* **How does the Dagger work?**

* **How will you choose between Dagger 2 and Dagger-Hilt?**

* **What is a Component in Dagger?**

* **What is Module in Dagger?**

* **How does the custom scope work in Dagger?**

* **When to call dispose and clear on CompositeDisposable in RxJava?** - [Learn from here](https://outcomeschool.com/blog/dispose-vs-clear-compositedisposable-rxjava)

* **What is Multipart Request in Networking?**

* **What is Flow in Kotlin?** - [Learn from here](https://outcomeschool.com/blog/flow-api-in-kotlin)

* **App Startup Library** - [Learn from here](https://outcomeschool.com/blog/app-startup-library)

* **Tell me something about RxJava.**

* **How will you handle error in RxJava?**

* **FlatMap Vs Map Operator** - [Learn from here](https://outcomeschool.com/blog/rxjava-map-vs-flatmap)
    
* **When to use `Create` operator and when to use `fromCallable` operator of RxJava?** - Learn from here: [RxJava Create and fromCallable Operator](https://outcomeschool.com/blog/rxjava-create-and-fromcallable-operator)
    
* **When to use `defer` operator of RxJava?** - Learn from here: [RxJava Defer Operator](https://outcomeschool.com/blog/rxjava-defer-operator)
    
* **How are Timer, Delay, and Interval operators used in RxJava?** - [Learn from here](https://outcomeschool.com/blog/rxjava-interval-operator)

* **How to make two network calls in parallel using RxJava?** - [RxJava Zip Operator](https://outcomeschool.com/blog/rxjava-zip-operator)
    
* **Tell the difference between Concat and Merge.** - [Learn from here](https://outcomeschool.com/blog/rxjava-concat-operator) and [here](https://outcomeschool.com/blog/rxjava-merge-operator)

* **Explain Subject in RxJava?** - [Learn from here](https://outcomeschool.com/blog/rxjava-subject-publish-replay-behavior-async)

* **What are the types of Observables in RxJava?** - Learn from here: [Types Of Observables In RxJava](https://outcomeschool.com/blog/types-of-observables-in-rxjava)

* **How to implement search feature using RxJava in your application?** - Learn from here: [Instant Search Using RxJava Operators](https://outcomeschool.com/blog/instant-search-using-rxjava-operators)

* **Pagination In RecyclerView Using RxJava Operators** - [Learn from here](https://outcomeschool.com/blog/pagination-in-recyclerview-using-rxjava-operators)

* **How The Android Image Loading Library Glide and Fresco Works?** - [Learn from here](https://outcomeschool.com/blog/android-image-loading-library-optimize-memory-usage), [here](https://outcomeschool.com/blog/android-image-loading-library-use-bitmap-pool-for-responsive-ui) and [here](https://outcomeschool.com/blog/android-image-loading-library-solve-the-slow-loading-issue)

* **Difference between Schedulers.io() and Schedulers.computation() in RxJava.**

### Android Architecture

Android Interview Questions and Answers:

* **Describe the architecture of your last app.**

* **Describe MVVM.** - [MVVM Architecture](https://outcomeschool.com/blog/mvvm-architecture-android)

* **MVC vs MVP vs MVVM architecture.**

* **Clean Architecture**

* **MVI** - [MVI (Model-View-Intent) Architecture in Android](https://www.linkedin.com/posts/amit-shekhar-iitbhu_outcomeschool-softwareengineering-tech-activity-7288428333430644738-muDc)

* **Software Architecture vs Software Design** - [Learn from here](https://www.linkedin.com/posts/outcomeschool_outcomeschool-softwareengineering-tech-activity-7230434583584858112-mMEG)

### Design Pattern

Android Interview Questions and Answers

* **Builder**
* **Singleton**
* **Factory**
* **Observer**
* **Repository**
* **Adapter**
* **Facade**
* **Dependency Injection**
* **Design Pattern used in Android** - [Learn from here](https://www.linkedin.com/posts/outcomeschool_outcomeschool-softwareengineering-tech-activity-7289501147243982848-hhym)
* **Kotlin Optional Parameters vs Builder Pattern** - [Learn from here](https://www.linkedin.com/posts/amit-shekhar-iitbhu_softwareengineer-androiddev-android-activity-7270656113845370881-LDW8)
* **Examples of the Observer pattern used in Android** - [Learn from here](https://www.linkedin.com/posts/amit-shekhar-iitbhu_androiddev-activity-7288114509120970752-Z6c8)

### Android System Design

Android Interview Questions and Answers:

Refer to this blog: [**Android System Design Interviews**](https://outcomeschool.com/blog/android-system-design-interviews) 

* **Design an Image Loading Library** - [Learn from here](https://outcomeschool.com/blog/android-image-loading-library-optimize-memory-usage), [here](https://outcomeschool.com/blog/android-image-loading-library-use-bitmap-pool-for-responsive-ui) and [here](https://outcomeschool.com/blog/android-image-loading-library-solve-the-slow-loading-issue)

* **Design File Downloader Library** - [Learn from here](https://github.com/amitshekhariitbhu/PRDownloader)

* **Design WhatsApp**

* **Design Instagram Stories**

* **Design Networking Library**

* **Design Facebook Near-By Friends App**

* **Design Caching Library.**

* **Design problems based on location-based app**

* **How to build an offline-first app? Explain the architecture**

* **Design LRU Cache**

* **Design Analytics Library**

* **HTTP Request vs HTTP Long-Polling vs WebSockets** - [Learn from blog](https://outcomeschool.com/blog/http-request-long-polling-websocket-sse) and [Video - HTTP Request vs HTTP Long-Polling vs WebSocket vs Server-Sent Events](https://www.youtube.com/watch?v=8ksWRX4xV-s)

* **How do Voice And Video Call Work?** - [Learn from here](https://outcomeschool.com/blog/voice-and-video-call)

* **Design Uber App** - [Learn from here](https://github.com/amitshekhariitbhu/ridesharing-uber-lyft-app)

* **Database Normalization vs Denormalization** - [Database Normalization vs Denormalization](https://outcomeschool.com/blog/database-normalization-vs-denormalization)

* **Hash vs Encrypt vs Encode** - [Learn from here](https://www.linkedin.com/posts/pallavi-shekhar_outcomeschool-softwareengineering-activity-7227173077665660929--KD8)

* **Webhook vs Polling** - [Learn from here](https://www.linkedin.com/posts/outcomeschool_softwareengineer-activity-7265962230553223168-fsPx)

* **Options for real-time updates in an Android App** - [Learn from here](https://www.linkedin.com/posts/amit-shekhar-iitbhu_androiddev-android-activity-7287460425212866560-dJNB)

* **Options for Network Optimization in a Mobile App** - [Options for Network Optimization in a Mobile App](https://www.linkedin.com/posts/outcomeschool_outcomeschool-softwareengineering-tech-activity-7287470994447900672-XYM9)

* **Firebase Remote Config in Android** - [Firebase Remote Config in Android](https://www.linkedin.com/posts/outcomeschool_outcomeschool-softwareengineering-tech-activity-7288408601944043520-pHZX)

### Android Unit Testing

Android Interview Questions and Answers:

* **Unit Testing ViewModel with Kotlin Coroutines and LiveData** - [Learn from here](https://outcomeschool.com/blog/unit-testing-viewmodel-with-kotlin-coroutines-and-livedata)

* **Unit Testing ViewModel with Kotlin Flow and StateFlow** - [Learn from here](https://outcomeschool.com/blog/unit-testing-viewmodel-with-kotlin-flow-and-stateflow)

* **What is Espresso?** - [Learn from here](https://developer.android.com/training/testing/espresso/basics)

* **What is Robolectric?** - [Learn from here](http://robolectric.org/)

* **What are the disadvantages of using Robolectric?** - [Learn from here](https://stackoverflow.com/questions/18271474/robolectric-vs-android-test-framework) 

* **What is UI-Automator?** - [Learn from here](https://developer.android.com/training/testing/ui-testing/uiautomator-testing.html)

* **Explain the unit test.** - [Learn from here](https://developer.android.com/training/testing/unit-testing/local-unit-tests)

* **Explain instrumented test.** - [Learn from here](https://developer.android.com/training/testing/unit-testing/instrumented-unit-tests)

* **Why Mockito is used?** - [Learn from here](http://site.mockito.org/)

* **Describe code coverage.**

### Android Tools And Technologies

Android Interview Questions and Answers:

* **What is ADB?** - [Learn from here](https://developer.android.com/studio/command-line/adb)

* **What is the StrictMode?** - Learn from here: [StrictMode](https://outcomeschool.com/blog/strictmode-in-android-development)

* **What is Lint? What is it used for?**

* **Android App Release Checklist For The Production Launch** - Learn from here: [Android App Release Checklist For The Production Launch](https://www.linkedin.com/posts/amit-shekhar-iitbhu_androiddev-android-activity-7275029928692080640-HIhx)

* **Git.**

* **Firebase.** - [Learn from here](https://firebase.google.com/)

* **How to measure method execution time in Android?**

* **Can you access your database of SQLite Database for debugging?** - [Learn from here](https://github.com/amitshekhariitbhu/Android-Debug-Database)

* **What are things that we need to take care while using Proguard?**

* **How to use Android Studio Memory Profiler?**

* **What is Kotlin DSL for Gradle?** - [Learn from here](https://www.linkedin.com/posts/amit-shekhar-iitbhu_softwareengineer-androiddev-android-activity-7282624364695404546-BvbS)

* **implementation vs api in Gradle** - [Learn from here](https://www.linkedin.com/posts/outcomeschool_outcomeschool-softwareengineering-tech-activity-7287325379441082368-_P9m)

* **What is Gradle?**

* **How do you create a custom task in Gradle?** - [Learn from here](https://www.linkedin.com/posts/amit-shekhar-iitbhu_softwareengineer-androiddev-android-activity-7282991795133685760-uUxE/)

* **APK Size Reduction.**

* **How can you speed up the Gradle build?**

* **About gradle build system.**

* **About multiple apk for android application.**

* **What is ProGuard used for?** - [Learn from here](https://www.linkedin.com/posts/amit-shekhar-iitbhu_outcomeschool-activity-7218840466283220993-afVr)

* **What is obfuscation? What is it used for? What about minification?**

* **How to change some parameters in an app without app update?**

* **What is Write-Ahead Logging (WAL) and why it is used internally in databases?** - [Learn from here](https://outcomeschool.com/blog/write-ahead-logging)

### Java

Android Interview Questions and Answers:

#### OOP

* **Explain OOP Concepts.**

* **Differences between abstract classes and interfaces?** 
    - An abstract class, is a class that contains both concrete and abstract methods 
    (methods without implementations). An abstract method must be implemented by the abstract class
     sub-classes. Abstract classes cannot be instantiated and need to be extended to be used.
    - An interface is like a blueprint/contract of a class (or it may be thought of as a class with methods, but without their implementation). It contains empty methods that 
    represent, what all of its subclasses should have in common. The subclasses provide the 
    implementation for each of these methods. Interfaces are implemented.

* **Difference between method overloading and overriding.**

* **What are the access modifiers you know? What does each one do?**
   - There are four access modifiers in Java language (from strictest to the most lenient):
        1. `private` *variables*, *methods*, *constructors* or *inner classes* are only visible to its' containing class and its' methods. This modifier is most commonly used, for example, to allow variable access only through getters and setters or to hide underlying implementation of classes that should not be used by user and therefore maintain encapsulation. Singleton constructor is also marked `private` to avoid unwanted instantiation from outside.
        2. `Default` (no keyword is used) this modifier can be applied to *classes*, *variables*, *constructors* and *methods* and allows access from classes and methods inside the same package.
        3. `protected` can be used on *variables*, *methods* and *constructors* therefore allowing access only to subclasses and classes that are inside the same package as protected members' class.
        4. `public` modifier is widely-used on *classes*, *variables*, *constructors* and *methods* to grant access from any class and method anywhere. It should not be used everywhere as it implies that data marked with `public` is not sensitive and can not be used to harm the program.

* **Can an Interface implement another Interface?**
  - Yes, an interface can implement another interface (and more than one), but it needs to use `extends`, rather than `implements` keyword. And while you can not remove methods from parent interface, you can add new ones freely to your sub-interface.

* **What is Polymorphism? What about Inheritance?**

#### Objects and Primitives

* **How is `String` class implemented? Why was it made immutable?**
  - There is no primitive variant of `String` class in Java language - all strings are just wrappers around underlying array of characters, which is declared `final`. This means that, once a `String` object is instantiated, it cannot be changed through normal tools of the language (Reflection still can mess things up horribly, because in Java no object is truly immutable). This is why `String` variables in classes are the first candidates to be used, when you want to override `hashCode()` and `equals()` of your class - you can be sure, that all their required contracts will be satisfied.
    > Note: The String class is immutable, so that once it is created a String object cannot be changed. The String class  has a number of methods, some of which will be discussed below, that appear to modify strings. Since strings are  immutable, what these methods really do is create and return a new string that contains the result of the operation. ([Official Java Documentation](https://docs.oracle.com/javase/tutorial/java/data/strings.html))

    This class is also unique in a sense, that, when you create an instance like this:
    ```java
    String helloWorld = "Hello, World!";
    ```
    `"Hello, World!"` is called a *literal* and compiler creates a `String` object with its' value. So
    ```java
    String capital = "Hello, World!".toUpperCase();
    ```
    is a valid statement, that, firstly, will create an object with literal value "Hello, World!" and then will create and return another object with value "HELLO, WORLD!"
  - `String` was made immutable to prevent malicious manipulation of data, when, for example, user login or other sensitive data is being send to a server.

* **What does it means to say that a `String` is immutable?**
    - It means that once created, `String` object's `char[]` (its' containing value) is declared `final` and, therefore, it can not be changed during runtime.

* **Can you list 8 primitive types in java?**
    - `byte`
    - `short`
    - `int`
    - `long`
    - `float`
    - `double`
    - `char`
    - `boolean`

* **What is the difference between an Integer and int?**
  - `int` is a primitive data type (with `boolean`, `byte`, `char`, `short`, `long`, `float` and `double`), while `Integer` (with `Boolean`, `Byte`, `Character`, `Short`,`Long`, `Float` and `Double`) is a [wrapper](https://docs.oracle.com/javase/tutorial/java/data/numberclasses.html) class that encapsulates primitive data type, while providing useful methods to perform different tasks with it.

* **Do objects get passed by reference or value in Java? Elaborate on that.**

#### Java Memory Model and Garbage Collector

* **What is garbage collector? How does it work?**
  - All objects are allocated on the heap area managed by the JVM.
  As long as an object is being referenced, the JVM considers it alive.
  Once an object is no longer referenced and therefore is not reachable by the application code,
  the garbage collector removes it and reclaims the unused memory.

#### Concurrency

* **What does the keyword `synchronized` mean?**

* **What is a `ThreadPoolExecutor`?** - [ThreadPoolExecutor in Android](https://outcomeschool.com/blog/threadpoolexecutor-in-android)

* **What is `volatile` modifier?**

* **Object Level Lock vs Class Level Lock in Java** - [Learn from here](https://x.com/amitiitbhu/status/1818156936413778332)

* **Concurrency vs Parallelism** - [Learn from here](https://www.linkedin.com/posts/pallavi-shekhar_outcomeschool-softwareengineering-activity-7226208648115404801-u8uu)

* **The classes in the atomic package expose a common set of methods: `get`, `set,`, `lazyset`, `compareAndSet`, and `weakCompareAndSet`. Please describe them.**

#### Exceptions

* **How does the `try{}`, `catch{}`, `finally` works?**

* **What is the difference between a `Checked Exception` and an `Un-Checked Exception`?**

#### Others

* **Shallow vs. Deep Copy in Java** - [Learn from here](https://www.linkedin.com/posts/amit-shekhar-iitbhu_outcomeschool-softwareengineering-activity-7224635014641016834-j8X1)

* **Explain Serialization and Deserialization** - [Learn from here](https://www.linkedin.com/posts/pallavi-shekhar_outcomeschool-softwareengineering-tech-activity-7228977637916823552-Bo2N)

* **What is serialization? How do you implement it?**

* **What is `transient` modifier?**

* **What are anonymous classes?**

* **What is the difference between using `==` and `.equals` on an object?**

* **What is the `hashCode()` and `equals()` used for?**

* **When would you make an object value `final`?**

* **What are these `final`, `finally` and `finalize` keywords?**

* **What is the difference between "throw" and "throws" keyword in Java?**
    - `throws` is just used to indicated which exception is to be thrown. But the `throw` keyword is used to throw some exception from any static block or any method.

* **What does the `static` word mean in Java?**
    - In case of `static` variable it means that this variable (its' value or the object it references) spans across all instances of enclosing class (changing it in one instance affects all others), while in case of `static` methods it means that these methods can be invoked without an instance of their enclosing class. It is useful, for example, when you create util classes that need not be instantiated every time you want to use them.

* **Can a `static` method be overridden in Java?**
    - While child class can override a static method with another static method with the same signature (return type can be down-casted), it is not truly overridden - it becomes "hidden", but both methods can still be accessed under right circumstances (see question about overloading/overriding above).

* **When is a `static` block run?**
    - Code inside static block is executed only once: the first time you make an object of that class or the first time you access a static member of that class (even if you never make an object of that class).

* **Explain Reflection in Java** - [Learn from here](https://x.com/amitiitbhu/status/1819234916812341567)

* **What is Dependency Injection?**

* **Difference between `StringBuffer` and `StringBuilder`?** - [Learn from here](https://outcomeschool.com/blog/string-vs-stringbuffer-vs-stringbuilder)

* **What is the difference between fail-fast and fail-safe iterators in Java?**

* **Monitor and Synchronization**

### Jetpack Compose

Topics you should know in **Jetpack Compose** for Android Interview:

* Compose
* State: remember, rememberSaveable, MutableState
* Recomposition
* State hoisting
* Side-effects
* Modifier
* Theme
* Layout, List
* Gestures, Animation
* CompositionLocal

Learn the above-mentioned from the following links:

- [Getting Started with Compose](https://developer.android.com/jetpack/compose/tutorial)
- [Thinking in Compose](https://developer.android.com/jetpack/compose/mental-model)
- [State](https://developer.android.com/jetpack/compose/state)
- [remember vs rememberSaveable](https://outcomeschool.com/blog/remember-vs-remembersaveable)
- [Lifecycle](https://developer.android.com/jetpack/compose/lifecycle)
- [Modifiers](https://developer.android.com/jetpack/compose/modifiers)
- [Side-effects](https://developer.android.com/jetpack/compose/side-effects)
- [Phases](https://developer.android.com/jetpack/compose/phases)
- [Semantics](https://developer.android.com/jetpack/compose/semantics)
- [CompositionLocal](https://developer.android.com/jetpack/compose/compositionlocal)
- [Can we use traditional Android Views and Compose together?](https://www.linkedin.com/posts/amit-shekhar-iitbhu_outcomeschool-softwareengineering-tech-activity-7235142707138961408-40hQ)

Questions

* **Jetpack Compose vs Android View System**
  
* **Explain the concept of declarative UI in Jetpack Compose.**
  
* **Declarative UI vs Imperative UI**
  
* **What are Composable functions?**
  
* **What is Recomposition?**
  
* **What is State in Compose?**
  
* **How does state management work in Jetpack Compose?**
  
* **Stateful composable vs Stateless composable**
  
* **What are the side effects?**
  
* **Difference between LaunchedEffect and DisposableEffect**.
  
* **What is rememberCoroutineScope and its use cases?**
  
* **How to observe Flows, and LiveData states in Compose UI?**
  
* **How can we handle asynchronous operations in Jetpack Compose?**
  
* **How can we convert a non-compose state into a Compose state?**
  
* **Explain derivedStateOf.**
  
* **Explain rememberUpdatedState.**
  
* **Difference between remember and rememberSaveable.**
  
* **Explain the Lifecycle of a Composable in Jetpack Compose.**
  
* **How do you handle lifecycle events in Compose functions?**
  
* **What are the best practices for performance optimization in Jetpack Compose?**
  
* **Can we use both Jetpack Compose and Android View in a Single App?**
  
* **What is State Hoisting?**
  
* **Explain CompositionLocal**
  
* **Explain Jetpack Compose Phases.**
  
* **What is the role of the Modifier in Jetpack Compose?**
  
* **What are Semantics?**
  
* **How can you handle user input and events in Jetpack Compose?**
  
* **How do you handle navigation in Jetpack Compose?**
  
* **How do you handle orientation changes in Jetpack Compose?**
  
* **Explain the concept of unidirectional data flow in Jetpack Compose.**
  
* **How to create Custom Layouts in Compose?**

### Other Topics

Android Interview Questions and Answers:

* **Describe SQLite.**

* **Have you used Room-Database?**

* **Can we identify the users who have uninstalled our application?**

* **Android Development Best Practices.** - Learn from here: [Android Development Best Practices](https://outcomeschool.com/blog/android-development-best-practices)

* **React Native vs Flutter** - Learn from here: [React Native vs Flutter](https://outcomeschool.com/blog/react-native-vs-flutter)

* **What are the metrics that you should measure continuously while android application development?** - Learn from here: [Android App Performance Metrics](https://outcomeschool.com/blog/android-app-performance-metrics)

* **How to avoid API keys from check-in into VCS?**

* **How does the Kotlin Multiplatform work?** - [Blog](https://outcomeschool.com/blog/how-does-the-kotlin-multiplatform-work)

* **How to use Memory Heap Dumps data?**

* **How to implement Dark Theme in your app?**

* **How to secure the API keys used in an Android App?**

* **What is Cleartext traffic?** Learn from here: [What is Cleartext traffic?](https://www.linkedin.com/posts/amit-shekhar-iitbhu_softwareengineer-androiddev-android-activity-7281879316601126913-x1az)

* **Tell something about memory usage in Android.**

* **Explain Annotation processing.**

* **How does the Android Push Notification system work?** Learn from here: [How does the Android Push Notification system work?](https://youtu.be/810IFG2sWlc)

* **Android Push Notification Flow using FCM.** Learn from here: [Android Push Notification Flow using FCM](https://outcomeschool.com/blog/android-push-notification-flow-using-fcm)

* **How to show local Notification at an exact time?**
