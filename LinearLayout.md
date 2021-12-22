###Hướng dẫn LinearLayout trong android

    <?xml version="1.0" encoding="utf-8"?>
    <LinearLayout android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:orientation="vertical"
        android:layout_margin="10dp"
        xmlns:android="http://schemas.android.com/apk/res/android">
    
        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content">
        <TextView
            android:id="@+id/textView1"
            android:textSize="20sp"
            android:layout_width="130dp"
            android:layout_height="wrap_content"
            android:text="Mã sinh viên:"/>
        <EditText
            android:id="@+id/editMaSV"
            android:layout_width="250dp"
            android:layout_height="wrap_content"
            android:textSize="16sp"/>
        </LinearLayout>
    
        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content">
            <TextView
                android:id="@+id/textView2"
                android:textSize="20sp"
                android:layout_width="130dp"
                android:layout_height="wrap_content"
                android:text="Tên sinh viên:"/>
            <EditText
                android:id="@+id/editTenSV"
                android:layout_width="250dp"
                android:layout_height="wrap_content"
                android:textSize="16sp"/>
        </LinearLayout>
    
        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content">
            <TextView
                android:id="@+id/textView3"
                android:textSize="20sp"
                android:layout_width="130dp"
                android:layout_marginTop="9dp"
                android:layout_height="wrap_content"
                android:text="Giới tính:"/>
                <RadioGroup
                    android:id="@+id/rggioitinh"
                    android:orientation="horizontal"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content">
                        <RadioButton
                            android:layout_marginRight="10dp"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:text="Nam"
                            android:checked="true"/>
                        <RadioButton
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:text="Nữ"/>
                </RadioGroup>
        </LinearLayout>
    
        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content">
            <TextView
                android:id="@+id/textView4"
                android:textSize="20sp"
                android:layout_width="130dp"
                android:layout_height="wrap_content"
                android:text="Ngày sinh:"/>
            <EditText
                android:id="@+id/editNgaySinh"
                android:layout_width="250dp"
                android:layout_height="wrap_content"
                android:textSize="16sp"/>
        </LinearLayout>
    
        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content">
    <Button
        android:id="@+id/btnThem"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_margin="15dp"
        android:text="THÊM"/>
        </LinearLayout>
        <TextView
            android:id="@+id/textView5"
            android:textSize="17sp"
            android:textStyle="bold"
            android:layout_width="200dp"
            android:layout_height="wrap_content"
            android:text="Danh sách sinh viên:"/>
    <ListView
        android:id="@+id/lvSinhVien"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"/>
    </LinearLayout>

demo
![](https://i0.wp.com/s1.uphinh.org/2021/12/22/imagefc6d00ac6d23215e.png)

##Item hiển thị ListView trong adapter

    <?xml version="1.0" encoding="utf-8"?>
    <LinearLayout android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="vertical"
        android:layout_margin="10dp"
        xmlns:android="http://schemas.android.com/apk/res/android">
        <LinearLayout
            android:layout_width="wrap_content"
            android:layout_height="wrap_content">
            <TextView
                android:id="@+id/textView1"
                android:textSize="20sp"
                android:layout_width="130dp"
                android:layout_height="wrap_content"
                android:text="Mã sinh viên:"
                android:textStyle="bold"/>
            <TextView
                android:id="@+id/txtMaSV"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="..."
                android:textSize="20sp"/>
        </LinearLayout>
        <LinearLayout
            android:layout_width="wrap_content"
            android:layout_height="wrap_content">
            <TextView
                android:id="@+id/textView2"
                android:textSize="20sp"
                android:layout_width="130dp"
                android:layout_height="wrap_content"
                android:text="Tên sinh viên:"
                android:textStyle="bold"/>
            <TextView
                android:id="@+id/txtTenSV"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="..."
                android:textSize="20sp"/>
        </LinearLayout>
    </LinearLayout>
