1. **Glide**
    > def version_glide = "4.11.0"
    > 
    > implementation "com.github.bumptech.glide:glide:$version_glide"
    > 
    > kapt "com.github.bumptech.glide:compiler:$version_glide"
    
2. **Room**
    > def room_version = "2.2.6"
    > 
    > implementation "androidx.room:room-runtime:$room_version"
    >
    > implementation "androidx.room:room-ktx:$room_version"
    > 
    > kapt "androidx.room:room-compiler:$room_version"
    
3. **Hilt**
    > def hilt_version = '2.33-beta'
    > 
    > implementation "com.google.dagger:hilt-android:$hilt_version"
    > 
    > kapt "com.google.dagger:hilt-compiler:$hilt_version"
    > 
    > implementation 'androidx.hilt:hilt-lifecycle-viewmodel:1.0.0-alpha03'
    > 
    > kapt 'androidx.hilt:hilt-compiler:1.0.0-beta01'
    
4. **Navigation**
    > def nav_version = "2.3.3"
    > 
    > implementation "androidx.navigation:navigation-fragment-ktx:$nav_version"
    > 
    > implementation "androidx.navigation:navigation-ui-ktx:$nav_version"
    
    
5. **Kotlin Coroutines**
    >implementation 'org.jetbrains.kotlinx:kotlinx-coroutines-core:1.4.2-native-mt'
    >
    >implementation 'org.jetbrains.kotlinx:kotlinx-coroutines-android:1.4.2-native-mt'
    
#Plugins

apply plugin: 'dagger.hilt.android.plugin'

apply plugin: "androidx.navigation.safeargs.kotlin"

classpath "com.google.dagger:hilt-android-gradle-plugin:$hilt_version"

def nav_version = "2.3.2"
classpath "androidx.navigation:navigation-safe-args-gradle-plugin:$nav_version"
