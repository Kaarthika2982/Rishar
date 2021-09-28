package com.example.rishar;

import androidx.appcompat.app.AppCompatActivity;

import android.content.Intent;
import android.os.Bundle;
import android.widget.Button;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        Button button1 = findViewById(R.id.button1);

        button1.setOnClickListener(view -> {
            Intent intent = new Intent(MainActivity.this, secondpage.class);
            startActivity(intent);
        });

        Button button2 = findViewById(R.id.button11);

        button2.setOnClickListener(view -> {
            Intent intent = new Intent(MainActivity.this, createaccount.class);
            startActivity(intent);
        });
    }
}


package com.example.rishar;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;

public class secondpage extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_secondpage);
    }
}


package com.example.rishar;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;

public class page3 extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_page3);
    }
}

