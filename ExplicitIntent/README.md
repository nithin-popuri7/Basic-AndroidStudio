
# Ex.No:2b Explicit Intents

Develop program to create two screens , first screen will take one number input from user. After click on Factorial button, second screen will open and it should display factorial of the same number using Explicit Intents.


## AIM:

To create a layout,click button and display factorial number using Explicit Intents in Android Studio.

## EQUIPMENTS REQUIRED:

Android Studio(Min. required Artic Fox)

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as ExplicitIntent and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display factorial number using Explicit Intents in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
Program to print the text “Explicit Intents”.
Developed by:P.Siva Naga Nithin
Registeration Number :212221240037
```

## MainActivity.java
~~~
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
    <EditText
        android:id="@+id/edt1"
        android:layout_width="350dp"
        android:layout_height="60dp"
        android:layout_centerHorizontal="true"
        android:hint="Enter a number"
        android:textAlignment="center"
        android:inputType="number"
        android:layout_marginTop="220dp"
        android:textStyle="bold"
        android:textSize="30sp"/>

    <Button
        android:id="@+id/btn1"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_below="@+id/edt1"
        android:layout_centerHorizontal="true"
        android:layout_marginTop="50dp"
        android:text="Factorial" />

</RelativeLayout>
~~~
## SecondActivity.java
~~~

package com.example.a2b;

import android.os.Bundle;
import android.widget.TextView;

import androidx.appcompat.app.AppCompatActivity;

public class SecondActivity extends AppCompatActivity {
    TextView txt2;

    @Override
    protected void onCreate(Bundle savedInstanceState) {

        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_second);

        Bundle b = getIntent().getExtras();

        int no = Integer.parseInt(b.getString("number"));
        long f=1;

        for(int i=no; i>0; i--)
        {
            f = f * i;
        }

        txt2 = findViewById(R.id.txt2);
        txt2.setText("Factorial of " + no + " is " + f);
    }

}
~~~
## activity.main_xml
~~~

<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
    <EditText
        android:id="@+id/edt1"
        android:layout_width="350dp"
        android:layout_height="60dp"
        android:layout_centerHorizontal="true"
        android:hint="Enter a number"
        android:textAlignment="center"
        android:inputType="number"
        android:layout_marginTop="220dp"
        android:textStyle="bold"
        android:textSize="30sp"/>

    <Button
        android:id="@+id/btn1"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_below="@+id/edt1"
        android:layout_centerHorizontal="true"
        android:layout_marginTop="50dp"
        android:text="Factorial" />

</RelativeLayout>
~~~

## activity_second.xml
~~~
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent">

    <TextView
        android:id="@+id/txt2"
        android:layout_width="500dp"
        android:layout_height="40dp"
        android:layout_centerHorizontal="true"
        android:layout_marginTop="40dp"
        android:textStyle="bold"
        android:textAlignment="center"
        android:textSize="30sp"
        />
</RelativeLayout>
~~~


## OUTPUT:

![2b 1](https://user-images.githubusercontent.com/94154780/190561268-46f652b7-f9fe-4d8f-acb2-b77885fc21b2.png)

![exp2b 1](https://user-images.githubusercontent.com/94154780/190561290-d322f6d6-5991-49d4-a4c6-0341953c543f.png)

![exp2b 2](https://user-images.githubusercontent.com/94154780/190561312-9076e837-35c1-4505-b438-1698296fe333.png)

![ex2b](https://user-images.githubusercontent.com/94154780/190659553-ae1feb38-138b-4726-9887-ee6f90589c6d.png)

![ex2b1](https://user-images.githubusercontent.com/94154780/190659666-1ef0c573-e2b3-46a4-b2d1-42fc0f2390a9.png)

![ex2b2](https://user-images.githubusercontent.com/94154780/190659493-07afe6aa-a2c3-44ed-9fda-a8ff2254cda9.png)

![exp2b 3](https://user-images.githubusercontent.com/94154780/190659756-1f94fa84-f73b-4664-821b-533bca1a70b1.png)

![exp2b 4](https://user-images.githubusercontent.com/94154780/190659785-3be03baa-d340-43b8-9ae2-dcefaf4d0fe0.png)

![exp2b 5](https://user-images.githubusercontent.com/94154780/190659886-fbdc8b26-1467-4b8e-8f92-8001cca027f1.png)









## RESULT
Thus a Simple Android Application to display factorial of the same number using Explicit Intents using Android Studio is developed and executed successfully.
