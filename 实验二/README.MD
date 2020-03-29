基本布局：

代码：

<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/Blue"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_margin="10dp"
        android:background="#00f"
        android:gravity="center"
        android:padding="25dp"
        android:text="BLUE"
        app:layout_constraintBottom_toTopOf="@+id/textView12"
        app:layout_constraintEnd_toEndOf="@+id/textView10"
        app:layout_constraintStart_toStartOf="@+id/textView10"
        app:layout_constraintTop_toBottomOf="@+id/textView10" />
    
    <TextView
        android:id="@+id/textView2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#f00"
        android:padding="25dp"
        android:text="RED"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />


    <TextView
        android:id="@+id/textView5"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#ffff00"
        android:padding="25dp"
        android:text="YELLOW"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
    
    <TextView
        android:id="@+id/textView7"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#0f0"
        android:padding="25dp"
        android:text="GREEN"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toStartOf="@+id/Blue"
    
        app:layout_constraintHorizontal_bias="0.9"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
    
    <TextView
        android:id="@+id/textView9"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#4b0082"
        android:padding="25dp"
        android:text="INDIGO"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.1"
        app:layout_constraintStart_toEndOf="@+id/Blue"
        app:layout_constraintTop_toTopOf="parent" />
    
    <TextView
        android:id="@+id/textView10"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#ffa500"
        android:padding="25dp"
        android:text="ORANGE"
        app:layout_constraintEnd_toStartOf="@+id/textView5"
        app:layout_constraintStart_toEndOf="@+id/textView2"
        app:layout_constraintTop_toTopOf="parent" />
    
    <TextView
        android:id="@+id/textView12"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:background="#ee82ee"
        android:gravity="center"
        android:padding="25dp"
        android:text="VIOLET"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>

![](./photo\1.png)

表格布局：

代码：

<?xml version="1.0" encoding="utf-8"?>
<TableLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:stretchColumns="1">
    <TableRow>
        <TextView
            android:layout_column="1"
            android:text="Open..."
            android:padding="3dip"/>
        <TextView
            android:gravity="right"
            android:text="Ctrl+O"
            android:padding="3dip"/>
    </TableRow>
    <TableRow>
    <TextView
        android:layout_column="1"
        android:text="Save..."
        android:padding="3dip"/>
    <TextView
        android:gravity="right"
        android:text="Ctrl+S"
        android:padding="3dip"/>
    </TableRow>
    <TableRow>
        <TextView
            android:layout_column="1"
            android:text="Save As..."
            android:padding="3dip"/>
        <TextView
            android:gravity="right"
            android:text="Ctrl+Shift+S"
            android:padding="3dip"/>
    </TableRow>
    <View
        android:layout_height="2dip"
        android:layout_width="match_parent"
        android:background="#66CCFF" />
    <TableRow>
        <TextView
            android:text="X"
            android:padding="3dip" />
        <TextView
            android:text="Import..."
            android:padding="3dip" />
    </TableRow>
    <TableRow>
        <TextView
            android:text="X"
            android:padding="3dip"/>
        <TextView
            android:text="Export..."
            android:padding="3dip"/>
    </TableRow>
    <View
        android:layout_height="2dp"
        android:layout_width="match_parent"
        android:background="#66CCFF" />
    <TableRow>
        <TextView
            android:layout_column="1"
            android:text="Quit"
            android:padding="3dp"/>
    </TableRow>
</TableLayout>

![](./photo\2.png)

线性布局：

代码：

<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:orientation="vertical"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:background="#FF909090">
    <LinearLayout android:layout_height="wrap_content"
        android:layout_width="match_parent">
        <TextView android:text="One,One"
            android:layout_height="wrap_content"
            android:layout_width="wrap_content"
            android:layout_margin="5dp"/>
        <TextView android:text="One,Two"
            android:layout_height="wrap_content"
            android:layout_width="wrap_content"
            android:layout_weight="1"
            android:layout_margin="5dp"
            android:gravity="center"/>
        <TextView android:text="One,Three"
            android:layout_height="wrap_content"
            android:layout_width="wrap_content"
            android:layout_margin="5dp"/>
        <TextView android:text="One,Four"
            android:layout_height="wrap_content"
            android:layout_width="wrap_content"
            android:layout_margin="5dp"/>
    </LinearLayout>
    <LinearLayout android:layout_height="wrap_content"
        android:layout_width="match_parent">
        <TextView android:text="Two,One"
            android:layout_height="wrap_content"
            android:layout_width="wrap_content"
            android:layout_margin="5dp"/>
        <TextView android:text="Two,Two"
            android:layout_height="wrap_content"
            android:layout_width="wrap_content"
            android:layout_weight="1"
            android:layout_margin="5dp"
            android:gravity="center"/>
        <TextView android:text="Two,Three"
            android:layout_height="wrap_content"
            android:layout_width="wrap_content"
            android:layout_margin="5dp"/>
        <TextView android:text="Two,Four"
            android:layout_height="wrap_content"
            android:layout_width="wrap_content"
            android:layout_margin="5dp"/>
    </LinearLayout>
    <LinearLayout android:layout_height="wrap_content"
        android:layout_width="match_parent">
        <TextView android:text="Three,One"
            android:layout_height="wrap_content"
            android:layout_width="wrap_content"
            android:layout_margin="5dp"/>
        <TextView android:text="Three,Two"
            android:layout_height="wrap_content"
            android:layout_width="wrap_content"
            android:layout_weight="1"
            android:layout_margin="5dp"
            android:gravity="center"/>
        <TextView android:text="Three,Three"
            android:layout_height="wrap_content"
            android:layout_width="wrap_content"
            android:layout_margin="5dp"/>
        <TextView android:text="Three,Four"
            android:layout_height="wrap_content"
            android:layout_width="wrap_content"
            android:layout_margin="5dp"/>
    </LinearLayout>
    <LinearLayout android:layout_height="wrap_content"
        android:layout_width="match_parent">
        <TextView android:text="Four,One"
            android:layout_height="wrap_content"
            android:layout_width="wrap_content"
            android:layout_margin="5dp"/>
        <TextView android:text="Four,Two"
            android:layout_height="wrap_content"
            android:layout_width="wrap_content"
            android:layout_weight="1"
            android:layout_margin="5dp"
            android:gravity="center"/>
        <TextView android:text="Four,Three"
            android:layout_height="wrap_content"
            android:layout_width="wrap_content"
            android:layout_margin="5dp"/>
        <TextView android:text="Four,Four"
            android:layout_height="wrap_content"
            android:layout_width="wrap_content"
            android:layout_margin="5dp"/>
    </LinearLayout>
</LinearLayout>

![](./photo\3.png)