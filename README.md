# Logger
A java logging tool that I enjoy working on
### Contributions
I love when people collaborate with me, feel free to pull request this repo when ever you like, I am open to all feedback as well!
### Use
Simply put this in your gradle file under repositories
```gradle
    maven { url 'https://jitpack.io' }
```
and this under your dependencies
```gradle
    implementation 'com.github.CoryRobertson:Logger:v1.0'
```
then in a class
```java
import com.github.coryrobertson.Logger.*;
```
and then somewhere in your code
```java
Logger.setLevel(LogLevels.LOG);
Logger.log("This message will be logged", LogLevels.LOG);
```
there are also LogLevels, at the moment, 4 called
- LogLevels.LOG
- LogLevels.WARN
- LogLevels.ERROR
- LogLevels.NONE

These levels are here so that only the Logger.level is printed to the console, all messages above and below the set log level are still sent to a file.
