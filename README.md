## Android Test Orchestrator bug

### Update: 
Switching from 

`androidTestImplementation 'com.android.support.test:orchestrator:1.0.2'`

to

`androidTestUtil 'com.android.support.test:orchestrator:1.0.2'`

solved the problem. This is even how it is described in the docs. :man_facepalming:


----------------


1. create brand new A/S project
2. see that AGP is set to 'com.android.tools.build:gradle:3.4.0-beta05'
3. add Android Test Orchestrator to project (not the AndroidX version)
4. start up an emulator
5. run the instrumentation test that was included in brand new project:
```
$ ./gradlew clean app:connectedDebugAndroidTest
```

6. see the tests fail:
> Task :app:connectedDebugAndroidTest FAILED
> 
> FAILURE: Build failed with an exception.
> 
> * What went wrong:
> Execution failed for task ':app:connectedDebugAndroidTest'.
> There were failing tests. See the report at: file:...../app/build/reports/androidTests/connected/index.html


7. open report and see: 
> No tests found. This usually means that your test classes are not in the form that your test runner expects (e.g. don't inherit from TestCase or lack @Test annotations).

8. look at the logs on the emulator. see [tombstone](tombstone.md)

```
JNI DETECTED ERROR IN APPLICATION: 
JNI NewGlobalRef called with pending exception java.lang.ClassNotFoundException: 
Didn't find class "android.support.test.services.shellexecutor.ShellMain" on path:...
```
