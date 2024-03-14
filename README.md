# Ex.No:2 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to print the text “Hello World”.
Developed by: PRAISEY S
Registeration Number : 212222040117
*/
```
## MainActivity.java
```
package com.example.exercise;

import android.os.Bundle;
import android.widget.Toast;
import androidx.appcompat.app.AppCompatActivity;


public class MainActivity extends AppCompatActivity {

    @Override

    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "Application Opened", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStart()
    {
        // It will show a message on the screen
        // then onStart is invoked
        super.onStart();
        Toast toast = Toast.makeText(getApplicationContext(), "Application Started", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onRestart() {
        // It will show a message on the screen
        // then onRestart is invoked
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(), "Restarted", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onResume() {
        // It will show a message on the screen
        // then onResume is invoked
        super.onResume();
        Toast toast = Toast.makeText(getApplicationContext(), "Application Resumed", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onPause() {
        // It will show a message on the screen
        // then onPause is invoked
        super.onPause();
        Toast toast = Toast.makeText(getApplicationContext(), "Application Paused", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStop() {
        // It will show a message on the screen
        // then onStop is invoked
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(), "On Soped", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onDestroy() {
        // It will show a message on the screen
        // then onDestroy is invoked
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
        toast.show();
    }
}
```

## activiy_main.xml
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        android:textColor="@android:color/holo_purple"
        android:textColorHighlight="@color/black"
        android:textSize="34sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.314" />

</androidx.constraintlayout.widget.ConstraintLayout>
```

## OUTPUT

![out 2 1](https://github.com/suryacse05/lifecyclemethods/assets/119394259/4ef83c0f-6a0c-4af6-af99-a581518f43c9)

![out 2 2](https://github.com/suryacse05/lifecyclemethods/assets/119394259/5f9c9993-d3dd-49f7-b776-53b73536496a)

![out 2 3](https://github.com/suryacse05/lifecyclemethods/assets/119394259/5c8d5961-7bd6-4cb4-a190-07505e749205)

![out 2 4](https://github.com/suryacse05/lifecyclemethods/assets/119394259/330dde8b-25ea-480c-a7ff-0f745aed41b3)

![out 2 5](https://github.com/suryacse05/lifecyclemethods/assets/119394259/c7866378-d4b1-47ca-b4b7-e2343fb6b6e7)


## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
