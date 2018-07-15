# android-ios
fully functional calculator


<?xml version="1.0" encoding="utf-8"?>
<android.support.constraint.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@color/colorPrimaryDark"
    tools:context=".MainActivity"
    tools:layout_editor_absoluteY="81dp">

    <EditText
        android:id="@+id/edit"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />


    <Button
        android:id="@+id/btn1"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginLeft="36dp"
        android:layout_marginStart="36dp"
        android:text="1"
        app:layout_constraintBaseline_toBaselineOf="@+id/btn2"
        app:layout_constraintStart_toStartOf="parent" />

    <Button
        android:id="@+id/btn2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="41dp"
        android:text="2"
        app:layout_constraintStart_toEndOf="@+id/btn1"
        app:layout_constraintTop_toBottomOf="@+id/edit" />

    <Button
        android:id="@+id/btn3"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="3"
        app:layout_constraintBaseline_toBaselineOf="@+id/btn2"
        app:layout_constraintStart_toEndOf="@+id/btn2" />

    <Button
        android:id="@+id/btnadd"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="add"
        app:layout_constraintBaseline_toBaselineOf="@+id/btnsub"
        app:layout_constraintStart_toStartOf="@+id/btn0" />

    <Button
        android:id="@+id/btn4"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="4"
        app:layout_constraintBaseline_toBaselineOf="@+id/btn5"
        app:layout_constraintStart_toStartOf="@+id/btn1" />

    <Button
        android:id="@+id/btn5"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="5"
        app:layout_constraintStart_toEndOf="@+id/btn1"
        app:layout_constraintTop_toBottomOf="@+id/btn1" />

    <Button
        android:id="@+id/btn6"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="6"
        app:layout_constraintBaseline_toBaselineOf="@+id/btn5"
        app:layout_constraintStart_toStartOf="@+id/btn3" />

    <Button
        android:id="@+id/btnsub"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="sub"
        app:layout_constraintStart_toEndOf="@+id/btn0"
        app:layout_constraintTop_toBottomOf="@+id/btn0" />

    <Button
        android:id="@+id/btn7"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="7"
        app:layout_constraintBaseline_toBaselineOf="@+id/btn8"
        app:layout_constraintStart_toStartOf="@+id/btn4" />

    <Button
        android:id="@+id/btn8"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="8"
        app:layout_constraintStart_toEndOf="@+id/btn4"
        app:layout_constraintTop_toBottomOf="@+id/btn4" />

    <Button
        android:id="@+id/btn9"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="9"
        app:layout_constraintBaseline_toBaselineOf="@+id/btn8"
        app:layout_constraintStart_toStartOf="@+id/btn6" />

    <Button
        android:id="@+id/btnmul"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="mul"
        app:layout_constraintBaseline_toBaselineOf="@+id/btnsub"
        app:layout_constraintStart_toEndOf="@+id/btnclear" />

    <Button
        android:id="@+id/btn0"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="0"
        app:layout_constraintBaseline_toBaselineOf="@+id/btnpoint"
        app:layout_constraintStart_toStartOf="@+id/btn7" />

    <Button
        android:id="@+id/btnpoint"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="46dp"
        android:text="."
        app:layout_constraintStart_toEndOf="@+id/btn7"
        app:layout_constraintTop_toTopOf="@+id/btn7" />

    <Button
        android:id="@+id/btnequal"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="="
        app:layout_constraintBaseline_toBaselineOf="@+id/btnpoint"
        app:layout_constraintStart_toStartOf="@+id/btn9" />

    <Button
        android:id="@+id/btndiv"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="div"
        app:layout_constraintStart_toEndOf="@+id/btnclear"
        app:layout_constraintTop_toBottomOf="@+id/btnmul" />

    <Button
        android:id="@+id/btnclear"
        android:layout_width="176dp"
        android:layout_height="wrap_content"
        android:text="clear"
        app:layout_constraintBaseline_toBaselineOf="@+id/btndiv"
        app:layout_constraintEnd_toEndOf="@+id/btnadd"
        app:layout_constraintStart_toEndOf="@+id/btnadd" />

</android.support.constraint.ConstraintLayout>



/*
* 
* mobile we app assignment
* assignment 5
* april 19 2018
*
*
*
* */

package com.example.ali.myapplication;

import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;



public class MainActivity extends AppCompatActivity {

    /*
    * Here we created reference for buttons and edit text
    *
    * */



    Button btn0, btn1, btn2, btn3, btn4, btn5, btn6,
            btn7, btn8, btn9, btnadd, btnsub, btndiv,
            btnmul, btnpoint, btnclear, btnequal;


    EditText edit;


    /*
     *Here we created two float variable for valueOne and valueTwo
     *
     * */




    float mValueOne, mValueTwo;


    /*
     * here we use boolean function for addition, substract, multiplication and division
     *
     * */


    boolean Addition, Subtract, Multiplication, Division;


    /*
     * here We override the method onCreate() that is the method of Activity class
     * */







    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);



        /*
         * here we declare each button by their ids on main activity
         *
         * */


        btn0 = (Button) findViewById(R.id.btn0);
        btn1 = (Button) findViewById(R.id.btn1);
        btn2 = (Button) findViewById(R.id.btn2);
        btn3 = (Button) findViewById(R.id.btn3);
        btn4 = (Button) findViewById(R.id.btn4);
        btn5 = (Button) findViewById(R.id.btn5);
        btn6 = (Button) findViewById(R.id.btn6);
        btn7 = (Button) findViewById(R.id.btn7);
        btn8 = (Button) findViewById(R.id.btn8);
        btn9 = (Button) findViewById(R.id.btn9);
        btnpoint = (Button) findViewById(R.id.btnpoint);
        btnadd = (Button) findViewById(R.id.btnadd);
        btnsub = (Button) findViewById(R.id.btnsub);
        btnmul = (Button) findViewById(R.id.btnmul);
        btndiv = (Button) findViewById(R.id.btndiv);
        btnclear = (Button) findViewById(R.id.btnclear);
        btnequal = (Button) findViewById(R.id.btnequal);
        edit = (EditText) findViewById(R.id.edit);




        /*
         * Here set onClickListener on Button0. If we click on Button0, EditText will display it.
         * we used the same logic for each button from 0 to 9
         *
         * */


        btn0.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                edit.setText(edit.getText() + "0");
            }
        });


        btn1.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                edit.setText(edit.getText() + "1");
            }
        });


        btn2.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                edit.setText(edit.getText() + "2");
            }
        });


        btn3.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                edit.setText(edit.getText() + "3");
            }
        });


        btn4.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                edit.setText(edit.getText() + "4");
            }
        });


        btn5.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                edit.setText(edit.getText() + "5");
            }
        });


        btn6.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                edit.setText(edit.getText() + "6");
            }
        });


        btn7.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                edit.setText(edit.getText() + "7");
            }
        });


        btn8.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                edit.setText(edit.getText() + "8");
            }
        });

        btn9.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                edit.setText(edit.getText() + "9");
            }
        });




        /*
        * Here first we have set the click listener on Add button. t
        * afterwards, Similarly we have set the click listener on other buttons i.e. sub,mul,div etc.
        *
        * */






        btnadd.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {

                if (edit == null) {
                    edit.setText("");
                } else {
                    mValueOne = Float.parseFloat(edit.getText() + "");
                    Addition = true;
                    edit.setText(null);
                }
            }
        });


        btnsub.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {

                if (edit == null) {
                    edit.setText("");
                } else {
                    mValueOne = Float.parseFloat(edit.getText() + "");
                    Subtract = true;
                    edit.setText(null);
                }
            }
        });


        btnmul.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {

                if (edit == null) {
                    edit.setText("");
                } else {
                    mValueOne = Float.parseFloat(edit.getText() + "");
                    Multiplication = true;
                    edit.setText(null);
                }
            }
        });


        btndiv.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {

                if (edit == null) {
                    edit.setText("");
                } else {
                    mValueOne = Float.parseFloat(edit.getText() + "");
                    Division = true;
                    edit.setText(null);
                }
            }
        });



        /**
         *
         * Here we put the if/else condition here, if Edittext is null then we set it as empty value,
         * else we add two values
         *
         * also set addition boolean value to true, which represents that add button is clicked and will be used when user click "=" button.
         *
         * we implement the same logic for subtract, multiplication and division.
         *
         * For each action, after the action is performs, then we set the value to false, so we can perform action again
         *
         * */



        btnequal.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                mValueTwo = Float.parseFloat(edit.getText() + "");

                if (Addition == true) {
                    edit.setText(mValueOne + mValueTwo + "");
                    Addition = false;
                }

                if (Subtract == true) {
                    edit.setText(mValueOne - mValueTwo + "");
                    Subtract = false;
                }

                if (Multiplication == true) {
                    edit.setText(mValueOne * mValueTwo + "");
                    Multiplication = false;
                }

                if (Division == true) {
                    edit.setText(mValueOne / mValueTwo + "");
                    Division = false;
                }
            }
        });



        btnclear.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                edit.setText("");
            }
        });

        btnpoint.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                edit.setText(edit.getText() + ".");
            }
        });
















    }
}

