<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:id="@+id/linearlayout"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    android:padding="16dp"
    android:layout_marginTop="10dp"
    android:background="#FAFAFA">

    <!-- Step 1: TextView for instructions -->
    <TextView
        android:id="@+id/tvInstructions"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="Enter your name, choose your country, and select an option below:"
        android:textSize="18sp"
        android:textColor="#000000"
        android:layout_marginBottom="16dp"
        android:textStyle="bold" />

    <!-- Step 2: EditText for user input -->
    <EditText
        android:id="@+id/etUserInput"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:hint="Enter your name"
        android:inputType="textPersonName"
        android:layout_marginBottom="16dp"
        android:ems="10" />

    <!-- Step 3: AutoCompleteTextView with sample country suggestions -->
    <AutoCompleteTextView
        android:id="@+id/autoCompleteCountry"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:hint="Select or type a country"
        android:inputType="text"
        android:layout_marginBottom="16dp"
        android:completionThreshold="1" />

    <!-- Step 4: Spinner with 5 sample options -->
    <Spinner
        android:id="@+id/spinnerOptions"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginBottom="20dp" />

    <!-- Optional TextView to display selected info -->
    <TextView
        android:id="@+id/tvResult"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text=""
        android:textSize="16sp"
        android:textColor="#333333"
        android:layout_marginTop="10dp" />

</LinearLayout>


package com.example.textcontrols;

import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.ArrayAdapter;
import android.widget.AutoCompleteTextView;
import android.widget.EditText;
import android.widget.Spinner;
import android.widget.TextView;

public class MainActivity extends AppCompatActivity {
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        // Step 2: EditText
        EditText etUserInput = findViewById(R.id.etUserInput);

        // Step 3: AutoCompleteTextView setup
        String[] countries = {"India", "USA", "Australia", "UK", "Italy", "Ireland", "South Africa"};
        AutoCompleteTextView autoCompleteCountry = findViewById(R.id.autoCompleteCountry);
        ArrayAdapter<String> countryAdapter = new ArrayAdapter<>(this,
                android.R.layout.simple_dropdown_item_1line, countries);
        autoCompleteCountry.setAdapter(countryAdapter);

        // Step 4: Spinner setup
        String[] options = {"Option 1", "Option 2", "Option 3", "Option 4", "Option 5"};
        Spinner spinnerOptions = findViewById(R.id.spinnerOptions);
        ArrayAdapter<String> spinnerAdapter = new ArrayAdapter<>(this,
                android.R.layout.simple_spinner_item, options);
        spinnerAdapter.setDropDownViewResource(android.R.layout.simple_spinner_dropdown_item);
        spinnerOptions.setAdapter(spinnerAdapter);
    }
}
