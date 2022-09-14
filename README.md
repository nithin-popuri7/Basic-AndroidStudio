### Basic-AndroidStudio
Developed:P.Siva Naga Nithin

Registered Number: 212221240037

### MainActivity.java
```
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
```

```
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
```

### OUTPUT
![onstart](https://user-images.githubusercontent.com/94154780/190152912-c3856c2c-6b24-46f1-8f8f-aba62824e131.png)
![onpause](https://user-images.githubusercontent.com/94154780/190154794-6f230618-8533-4364-b769-ed79b8c251fd.png)
![oncreate](https://user-images.githubusercontent.com/94154780/190153068-c048fd90-baa6-482b-9512-f0dcbfb3c74b.png)
![ondestroy](https://user-images.githubusercontent.com/94154780/190153128-dd07708b-172d-4b53-89cd-839c586bdc77.png)
![onresume](https://user-images.githubusercontent.com/94154780/190153184-9d26c5e2-db43-4ec7-bb14-aa313bd7de15.png)
![onrestart](https://user-images.githubusercontent.com/94154780/190153212-e775bd1c-5fbf-4114-97b5-e05b578064a3.png)
![onstop](https://user-images.githubusercontent.com/94154780/190153933-b4a93d11-c85a-45a2-9ab0-a41750ca40d3.png)





### Result

Therefore a program is return to develop a program to detect the various life cycles of an activity. The program is successfully executed.




