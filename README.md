# Shining_Angels
Android Project
//Java codes for ListView
package com.example.lenovo.listview;

import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.ArrayAdapter;
import android.widget.ListView;

import java.util.ArrayList;

import static com.example.lenovo.listview.R.*;

public class MainActivity extends AppCompatActivity {


    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(layout.activity_main);
    ListView  listView=(ListView) findViewById(R.id.listview);
        ArrayList<String> arraylist = new ArrayList<String>();
        arraylist.add("Abhay");
        arraylist.add("Satyam");
        arraylist.add("Rushi");
        arraylist.add("Kiran");
        arraylist.add("Bhaskar");
        arraylist.add("Manish");
        arraylist.add("Rakesh");
        arraylist.add("Abhishek");
        arraylist.add("Ram");
        arraylist.add("Vinay");
        arraylist.add("Faiz");
        arraylist.add("African");
        ArrayAdapter<String> itemsAdapter =
                new ArrayAdapter<String>(this,R.layout.activity_listview, arraylist);

        listView.setAdapter(itemsAdapter);











    }
}
