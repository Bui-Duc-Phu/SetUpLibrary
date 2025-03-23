# Hilt Android (Jetpack Compose)

<h2>
step 1: Thêm Dependencies (yêu cầu hoàn thành theo các bước)
<h2>
Mở file build.gradle.kts (Module: app) và thêm các dependencies sau:

<pre>
<code>
plugins {
    alias(libs.plugins.android.application)
    alias(libs.plugins.kotlin.android)
    alias(libs.plugins.kotlin.compose)

  //thêm kapt sau đó sync 
    kotlin("kapt")
  
}
</code>
</pre>

step 2: Trong phần dependencies:

<pre>
<code>
dependencies {
    // thêm và sync
    <!-- Hilt Core -->
    implementation("com.google.dagger:hilt-android:2.51.1")
    kapt("com.google.dagger:hilt-android-compiler:2.51.1")
    <!-- Hilt cho ViewModel -->
    implementation("androidx.hilt:hilt-lifecycle-viewmodel:1.0.0-alpha03")
    kapt("androidx.hilt:hilt-compiler:1.2.0")
}
</code>
</pre>

step 3: Cấu hình Gradle

Mở file build.gradle.kts (Project) và thêm:
    // thêm và sync
<pre>
<code>
buildscript {
    dependencies {
        classpath("com.google.dagger:hilt-android-gradle-plugin:2.51.1")
    }
}
</code>
</pre>

step 4: Cấu hình Gradle

Mở file build.gradle.kts (Module: app) và thêm các dependencies sau:

<pre>
<code>
plugins {
    alias(libs.plugins.android.application)
    alias(libs.plugins.kotlin.android)
    alias(libs.plugins.kotlin.compose)
    kotlin("kapt")

  // thêm và sync
     id("com.google.dagger.hilt.android")
  
}
</code>
</pre>




# Viewmodel setup (Jetpack Compose)
1. Thêm Dependencies
<pre>
<code>
    //viewmodel
    implementation("androidx.lifecycle:lifecycle-viewmodel-compose:2.8.7")
    implementation("androidx.lifecycle:lifecycle-viewmodel-savedstate:2.8.7")
    implementation("androidx.lifecycle:lifecycle-runtime-ktx:2.8.7")
    implementation("androidx.lifecycle:lifecycle-viewmodel-ktx:2.8.7")
</code>
</pre>




# Retrofit setup (Jetpack Compose)
1. Thêm Dependencies
<pre>
<code>
     // Retrofit core library
    implementation("com.squareup.retrofit2:retrofit:2.11.0")
    implementation("com.squareup.retrofit2:converter-gson:2.11.0")
    implementation("com.squareup.okhttp3:logging-interceptor:4.11.0")
    implementation("com.squareup.okhttp3:okhttp:4.11.0")
</code>
</pre>


# Room setup (Jetpack Compose)
1. Thêm Dependencies
<pre>
<code>
    //room
    implementation("androidx.room:room-runtime:2.6.1")
    kapt("androidx.room:room-compiler:2.6.1")
</code>
</pre>


# Paging3 setup (Jetpack Compose)
1. Thêm Dependencies
<pre>
<code>
  //paging3
  implementation("androidx.paging:paging-compose:3.3.6")
</code>
</pre>


# Navigation setup (Jetpack Compose)
1. Thêm Dependencies
<pre>
<code>
    //navigation
    implementation("androidx.navigation:navigation-compose:2.8.7")
</code>
</pre>

# viewpager setup (Jetpack Compose)
1. Thêm Dependencies
<pre>
<code>
    //viewpager
    implementation("com.google.accompanist:accompanist-pager:0.32.0")
</code>
</pre>

</pre>

# viewpager setup (Jetpack Compose)
1. Thêm Dependencies
<pre>
<code>
    //viewpager
    implementation("com.google.accompanist:accompanist-pager:0.32.0")
</code>
</pre>


# Preview setup (Jetpack Compose)
1. Thêm Dependencies
<pre>
<code>
    //Preview
    implementation("androidx.compose.ui:ui-tooling-preview:1.7.8") // Phiên bản mới nhất
    debugImplementation("androidx.compose.ui:ui-tooling:1.7.8")
    implementation("androidx.compose.ui:ui-graphics:1.7.8") //
</code>
</pre>

















