### Basic-AndroidStudio
Developed:P.SIva Naga Nithin

Registered Number: 212221240037

### MainActivity.java

package com.example.exp1;
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.Toast;
public class MainActivity extends AppCompatActivity {
  @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);




        Toast toast = Toast.makeText(getApplicationContext(), "OnCreate Executed", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStart(){
        super.onStart();
        Toast toast=Toast.makeText(getApplicationContext(),"OnStart Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onResume(){
        super.onResume();
        Toast toast=Toast.makeText(getApplicationContext(),"OnResume Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onPause(){
        super.onPause();
        Toast toast=Toast.makeText(getApplicationContext(),"OnPause Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStop(){
        super.onStop();
        Toast toast=Toast.makeText(getApplicationContext(),"OnStop Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onRestart(){
        super.onRestart();
        Toast toast=Toast.makeText(getApplicationContext(),"OnRestart Executed",Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onDestroy(){
        super.onDestroy();
        Toast toast=Toast.makeText(getApplicationContext(),"OnDestroy Executed",Toast.LENGTH_LONG);
        toast.show();
    }
}

### activity_main.xml

<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="HelloWorld!"
        android:layout_centerVertical="true"
        android:layout_centerHorizontal="true"
        android:textSize="20sp"
        android:textColor="@color/black"

        />
</RelativeLayout>

### OUTPUT
[exp1](https://user-images.githubusercontent.com/94154780/190052416-25a54867-0c4b-42b5-af15-e62311575004.png)
![exp1 1](https://user-images.githubusercontent.com/94154780/190052455-49660791-aa68-4744-895d-d71ca3e0833b.png)
![exp1 2](https://user-images.githubusercontent.com/94154780/190052471-3ecc6c72-9a2a-448a-b187-8d5bf0!
[exp1 3](https://user-images.githubusercontent.com/94154780/190052488-8be2c88c-bf44-4ce7-8db5-79773331137c.png)
66af3f.png)
![exp1 4](https://user-images.githubusercontent.com/94154780/190052516-966839c6-5648-4cf0-ac9f-9dd28f100d9f.png)
![exp1 5](https://user-images.githubusercontent.com/94154780/190052552-7416c3dc-9aef-45dc-9d60-1d2316c060d5.png)
![exp1 6](https://user-images.githubusercontent.com/94154780/190052576-444c9655-e5ca-449c-9327-01983990c269.png)




