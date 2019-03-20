# MainActivityLife
实验目的：验证Activity的生命周期<br>
截图：<br>
![image](https://github.com/wrh0619/hellowworld/blob/master/app/src/main/res/layout/hello1.JPG)
![image](https://github.com/wrh0619/hellowworld/blob/master/app/src/main/res/layout/hello2.JPG)
关键代码：
```
package com.example.hellowworld;


import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.util.Log;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        //setContentView(R.layout.layout11);
        Log.i("MainActivityLife","调用onCreate()");
        setContentView(R.layout.activity_main);
        //setContentView(R.layout.relative);
    }
    @Override
    protected void onStart(){
        super.onStart();
        Log.i("MainActivityLife","调用onstart()");
    }
    @Override
    protected void onResume(){
        super.onResume();
        Log.i("MainActivityLife","调用onresume()");
    }
    @Override
    protected void onPause() {
        super.onPause();
        Log.i("MainActivityLife","调用onpause()");
    }
    @Override
    protected void onStop() {
        super.onStop();
        Log.i("MainActivityLife","调用onstop()");
    }
    @Override
    protected void onDestroy() {
        super.onDestroy();
        Log.i("MainActivityLife","调用ondestroy()");
    }
    protected void onRestart() {
        super.onRestart();
        Log.i("MainActivityLife","调用onRestart()");
    }
}
```
