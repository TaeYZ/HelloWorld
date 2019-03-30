# 安卓移动开发试验一：HelloWorld

## 一、试验内容
通过Android studio，实现HelloWorld
## 二、试验代码与截图
layout代码：
```
<?xml version="1.0" encoding="utf-8"?>
<android.support.constraint.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</android.support.constraint.ConstraintLayout>
```
activity代码：
```
package com.example.helloworld;

import android.nfc.Tag;
import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.util.Log;

public class MainActivity extends AppCompatActivity {
    public static final  String TAG="MainActivity";
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Log.e(TAG,"onCreate!");
    }
    @Override
    protected void onStart() {
        super.onStart();
        Log.e(TAG,"onStart!");
    }
    @Override
    protected void onResume() {
        super.onResume();
        Log.e(TAG,"onResume!");
    }
    @Override
    protected void onPause() {
        super.onPause();
        Log.e(TAG,"onPause!");
    }
    @Override
    protected void onStop() {
        super.onStop();
        Log.e(TAG,"onStop!");
    }
    @Override
    protected void onDestroy() {
        super.onDestroy();
        Log.e(TAG,"onDestroy!");
    }
}
```

截图：

![HelloWorld](https://img-blog.csdnimg.cn/20190318145217728.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2h1YWlxaTgzNzg=,size_16,color_FFFFFF,t_70)

![activity](https://img-blog.csdnimg.cn/20190330164601383.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2h1YWlxaTgzNzg=,size_16,color_FFFFFF,t_70)
