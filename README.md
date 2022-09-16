### Basic-AndroidStudio
```
## Developed:P.Siva Naga Nithin
## Registered Number: 212221240037
```
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

 ### activity_main.xml
 ```

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

### OUTPUT:
![exp1](https://user-images.githubusercontent.com/94154780/190669055-de4de347-296a-412d-8a5c-93759fd540a1.png)


![oncreate](https://user-images.githubusercontent.com/94154780/190668980-43f432e6-6b6e-47cd-ae9e-cc2bc3c884fe.png)

![onstap](https://user-images.githubusercontent.com/94154780/190669157-bed6a110-9f14-4497-b598-89159c4ba2d5.png)

![onrestart](https://user-images.githubusercontent.com/94154780/190669241-4e1fece2-d239-4cfd-9ac6-3187d9824022.png)

![onresume](https://user-images.githubusercontent.com/94154780/190669292-8bb0a61a-7790-4889-9b59-771d9798a76c.png)

![onpause](https://user-images.githubusercontent.com/94154780/190669327-36f85fca-19ad-46d2-ad9a-6145d6712cd6.png)

![ondestroy](https://user-images.githubusercontent.com/94154780/190669502-35a3023a-9a3f-44e4-8ddf-32cd42162c2a.png)

![onstart](https://user-images.githubusercontent.com/94154780/190669585-655edd7e-eeca-4821-8019-3754bb424bed.png)














### Result

Therefore a program is return to develop a program to detect the various life cycles of an activity. The program is successfully executed.




