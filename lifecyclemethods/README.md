# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.

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
Developed by:teja
Registeration Number :212221040067
*/
XML-CODE :
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
xmlns:android="http://schemas.android.com/apk/res/android"
xmlns:app="http://schemas.android.com/apk/res-auto"
xmlns:tools="http://schemas.android.com/tools"
android:layout_width="match_parent"
android:layout_height="match_parent"
tools:context=".MainActivity">
<TextView
android:id="@+id/textView"
android:layout_width="334dp"
android:layout_height="96dp"
android:layout_marginStart="90dp"
android:layout_marginTop="286dp"
android:text="LIFE CYCLE"
android:textColor="#673AB7"
android:textSize="36sp"
app:layout_constraintStart_toStartOf="parent"
app:layout_constraintTop_toTopOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>
Main Activity :
package com.example.androidlifecycle;
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.Toast;
public class MainActivity extends AppCompatActivity {
@Override
protected void onCreate(Bundle savedInstanceState) {
super.onCreate(savedInstanceState);
setContentView(R.layout.activity_main);
Toast toast =
Toast.makeText(getApplicationContext(),"Oncreate",Toast.LENGTH_SHORT);
toast.show();
}
protected void onStart(){
super.onStart();
Toast toast =
Toast.makeText(getApplicationContext(),"Onstart",Toast.LENGTH_SHORT);
toast.show();
}
9/19/23, 1:24 PM Mobile-Application-Development/lifecyclemethods/README.md at b41b2d6683cbdd1b09f75d340b2092388aea82f9 · Sudhin…
https://github.com/Sudhindev/Mobile-Application-Development/blob/b41b2d6683cbdd1b09f75d340b2092388aea82f9/lifecyclemethods/README.… 3/4
protected void onPause(){
super.onPause();
Toast toast =
Toast.makeText(getApplicationContext(),"Onpause",Toast.LENGTH_SHORT);
toast.show();
}
protected void onResume(){
super.onResume();
Toast toast =
Toast.makeText(getApplicationContext(),"onResume",Toast.LENGTH_SHORT);
toast.show();
}
protected void onStop(){
super.onStop();
Toast toast =
Toast.makeText(getApplicationContext(),"OnStop",Toast.LENGTH_SHORT);
toast.show();
}
protected void onDestroy(){
super.onDestroy();
Toast toast =
Toast.makeText(getApplicationContext(),"onDestroy",Toast.LENGTH_SHORT);
toast.show();
}
protected void onRestart(){
super.onRestart();
Toast toast =
Toast.makeText(getApplicationContext(),"onRestart",Toast.LENGTH_SHORT);
toast.show();
}
}
```

## OUTPUT
![image](https://github.com/suryacse05/Mobile-Application-Development/assets/151063592/db9ae1b2-0a7a-4880-923d-64df3ab6a759)

## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
