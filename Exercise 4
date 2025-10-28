<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:id="@+id/l_layout"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    android:gravity="center_horizontal"
    android:padding="20dp"
    android:background="#F2F2F2">

    <!-- Standard Button -->
    <Button
        android:id="@+id/standardButton"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Standard Button"
        android:layout_marginTop="40dp"
        android:onClick="onStandardButtonClick" />

    <!-- Image Button -->
    <ImageButton
        android:id="@+id/imageButton"
        android:layout_width="100dp"
        android:layout_height="100dp"
        android:layout_marginTop="40dp"
        android:contentDescription="Image Button"
        android:background="@android:color/transparent"
        android:src="@drawable/ic_launcher_foreground"
        android:onClick="onImageButtonClick" />

    <!-- Toggle Button -->
    <ToggleButton
        android:id="@+id/toggleButton"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="40dp"
        android:textOn="Switch ON"
        android:textOff="Switch OFF"
        android:checked="false"
        android:onClick="onToggleButtonClick" />

</LinearLayout>


package com.tutlane.buttonexample;

import android.os.Bundle;
import android.view.View;
import android.widget.ImageButton;
import android.widget.Button;
import android.widget.ToggleButton;
import android.widget.Toast;
import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }

    // Step 2 & 3: Event Handlers with Toast messages
    public void onStandardButtonClick(View view) {
        Toast.makeText(getApplicationContext(), "Standard Button Clicked", Toast.LENGTH_SHORT).show();
    }

    public void onImageButtonClick(View view) {
        Toast.makeText(getApplicationContext(), "Image Button Clicked", Toast.LENGTH_SHORT).show();
    }

    public void onToggleButtonClick(View view) {
        ToggleButton toggle = (ToggleButton) view;
        if (toggle.isChecked()) {
            Toast.makeText(getApplicationContext(), "Toggle is ON", Toast.LENGTH_SHORT).show();
        } else {
            Toast.makeText(getApplicationContext(), "Toggle is OFF", Toast.LENGTH_SHORT).show();
        }
    }
}
