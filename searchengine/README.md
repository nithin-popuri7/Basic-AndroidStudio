# Ex.No:6 Build a program to create a first display screen of any search engine using Auto Complete Text View.

## AIM:

To develop a program to create a first display screen of any search engine using AutoComplete TextView in Android Studio.

## EQUIPMENTS REQUIRED:

Android Studio(Min.required Artic Fox)

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as searchengine and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout using AutoComplete TextView in activity_main.xml.

Step 6: Display screen of search engine in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
Developed by:P.Siva Naga Nithin
Registeration Number:212221240037
```
### Program to print the text “display screen of any search engine”.
### Main Activity.java:
```
package com.example.nithinautocompletetextview;
import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.ArrayAdapter;
import android.widget.AutoCompleteTextView;

public class MainActivity extends AppCompatActivity {
    AutoCompleteTextView autocomplete;

    String[] arr = { "Bing","Google","Yandex","Yahoo","DuckDuckGo","Swisscows","StartPage","Gibiru"};

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        autocomplete = (AutoCompleteTextView)
                findViewById(R.id.autoCompleteTextView1);

        ArrayAdapter<String> adapter = new ArrayAdapter<String>
                (this,android.R.layout.select_dialog_item, arr);

        autocomplete.setThreshold(2);
        autocomplete.setAdapter(adapter);
    }
}
```
### strings.xml:
```
<resources>
    <string name="app_name">within.autocompleting</string>
    <string name="search">search</string>
</resources>
```
### activity_main.xml:
```
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#32D5D5"
    android:padding="5dp"
    tools:context=".MainActivity">


    <AutoCompleteTextView
        android:id="@+id/autoCompleteTextView1"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_below="@+id/textView2"
        android:layout_centerHorizontal="true"
        android:layout_marginStart="30dp"
        android:layout_marginTop="30dp"
        android:layout_marginEnd="30dp"
        android:layout_marginBottom="30dp"
        android:ems="10"
        android:hint="@string/search"
        android:textAlignment="center"
        tools:ignore="UnknownId" />

</RelativeLayout>
```


## OUTPUT:
![exp6](https://user-images.githubusercontent.com/94154780/199955182-cfd84231-0472-4648-ad7e-ad3e13c5abad.png)

![exp6 1](https://user-images.githubusercontent.com/94154780/199955205-4fd146b7-b3b9-4023-9cfc-5ffba164ec8c.png)

![ex6 2](https://user-images.githubusercontent.com/94154780/199955245-f46801b0-b14c-4613-bc57-60cd2f5b3173.png)

![ex6 3](https://user-images.githubusercontent.com/94154780/199955290-422b7a17-a44a-45ba-8d2f-60146f8faa52.png)

![exp6 4](https://user-images.githubusercontent.com/94154780/199955326-941c1e3c-6a05-44a2-b38a-4fb359efdd3d.png)



## RESULT
Thus a Simple Android Application develop a program to create a first display screen of any search engine using AutoComplete TextView in Android Studio is developed and executed successfully.
