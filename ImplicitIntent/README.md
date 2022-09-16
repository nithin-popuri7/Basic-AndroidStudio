
# Ex.No:2a Implicit Intent

Develop program to create a text field and a button “Navigate”. When you enter “www.google.com” and press navigate button it should open google page using Implicit Intents.


## AIM:

To create a layout,click button,open google page using Implicit Intents in Android Studio.

## EQUIPMENTS REQUIRED:

Android Studio(Min. required Artic Fox)

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as ImplicitIntent and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: open google page using Implicit Intents in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
~~~
Program to print the text “Implicit Intent”.
Developed by:P.Siva Naga Nithin
Registeration Number :212221240037
~~~
## MainActivity.java
~~~
package com.example.ex2a.;
import androidx.appcompat.app.AppCompatActivity;
import android.content.Intent;
import android.os.Bundle;
import android.widget.Button;
import android.widget.EditText;
import android.net.Uri;

public class MainActivity extends AppCompatActivity {
    EditText edit1;
    Button Button1;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        edit1 = findViewById(R.id.edit1);
        Button1 = findViewById(R.id.Button1);

        Button1.setOnClickListener(view ->{
            String  url = edit1.getText().toString();
            Intent intent = new Intent(Intent.ACTION_VIEW,Uri.parse(url));
            startActivity(intent);
        });

    }
}
~~~
## activity_main.xml
~~~

package com.example.exp2;

import androidx.appcompat.app.AppCompatActivity;

import android.content.Intent;
import android.os.Bundle;
import android.widget.Button;
import android.widget.EditText;
import android.net.Uri;

public class MainActivity extends AppCompatActivity {
        EditText edit1;
        Button Button1;

        @Override
        protected void onCreate(Bundle savedInstanceState) {
                super.onCreate(savedInstanceState);
                setContentView(R.layout.activity_main);
                edit1 = findViewById(R.id.edit1);
                Button1 = findViewById(R.id.Button1);

                Button1.setOnClickListener(view ->{
                        String  url = edit1.getText().toString();
                        Intent intent = new Intent(Intent.ACTION_VIEW,Uri.parse(url));
                        startActivity(intent);
                });

        }
}

~~~
## OUTPUT

![exp2a](https://user-images.githubusercontent.com/94154780/190657156-5e5fecba-71bc-48c7-9298-62a2899010e4.png)

![expl](https://user-images.githubusercontent.com/94154780/190681643-2bf42980-e02d-40ea-a31d-72be3ab4ffac.png)

![exp2a2](https://user-images.githubusercontent.com/94154780/190657636-2a5aec9b-e18a-41f3-a327-6ecdf4cca186.png)

![Ex2a3](https://user-images.githubusercontent.com/94154780/190679989-12f0e5bd-3e30-446f-a13e-3a6084a02fca.png)

![expl1](https://user-images.githubusercontent.com/94154780/190682818-1f40d378-7c68-41d4-a462-c356699dcd4d.png)





## RESULT
Thus a Simple Android Application to open google page using Implicit Intents using Android Studio is developed and executed successfully.
