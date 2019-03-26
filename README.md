# Android实验二
## Android布局
### LinearLayout，ConstraintLayout，TableLayout的使用
#### 1.利用线性布局实现如下界面
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190326103425131.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyMjQxNDEy,size_16,color_FFFFFF,t_70)
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:paddingLeft="5dp"
    android:paddingRight="5dp"
    android:background="#000000"
    android:orientation="vertical">
    <LinearLayout
        android:layout_width="370dp"
        android:layout_height="wrap_content"
        android:orientation="horizontal">
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="One,One"
            android:textColor="#FFFFFF"/>
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="One,Two"
            android:textColor="#FFFFFF"/>
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="One,Three"
            android:textColor="#FFFFFF"/>
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="One,Four"
            android:textColor="#FFFFFF"/>
    </LinearLayout>
    <LinearLayout
        android:layout_width="370dp"
        android:layout_height="wrap_content"
        android:orientation="horizontal">
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="Two,One"
            android:textColor="#FFFFFF"/>
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="Two,Two"
            android:textColor="#FFFFFF"/>
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="Two,Three"
            android:textColor="#FFFFFF"/>
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="Two,Four"
            android:textColor="#FFFFFF"/>
    </LinearLayout>
    <LinearLayout
        android:layout_width="370dp"
        android:layout_height="wrap_content"
        android:orientation="horizontal">
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="Three,One"
            android:textColor="#FFFFFF" />
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="Three,Two"
            android:textColor="#FFFFFF"/>
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="Three,Three"
            android:textColor="#FFFFFF"/>
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="Three,Four"
            android:textColor="#FFFFFF"/>
    </LinearLayout>
    <LinearLayout
        android:layout_width="370dp"
        android:layout_height="wrap_content"
        android:orientation="horizontal">
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="Four,One"
            android:textColor="#FFFFFF"/>
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="Four,Two"
            android:textColor="#FFFFFF"/>
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="Four,Three"
            android:textColor="#FFFFFF"/>
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="Four,Four"
            android:textColor="#FFFFFF"/>
    </LinearLayout>
</LinearLayout>
![在这里插入图片描述](https://img-blog.csdnimg.cn/2019032610414965.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyMjQxNDEy,size_16,color_FFFFFF,t_70)
#### 2.利用ConstraintLayout实现如下界面：
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190326103537418.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyMjQxNDEy,size_16,color_FFFFFF,t_70)
<android.support.constraint.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="250dp"
    android:background="#000000">
    <Button
        android:id="@+id/B1"
        android:layout_width="90dp"
        android:layout_height="wrap_content"
        android:background="#DC143C"
        android:text="RED" />
    <Button
        android:id="@+id/B2"
        android:layout_width="90dp"
        android:layout_height="wrap_content"
        android:background="#FFA500"
        android:text="Orange"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent" />
    <Button
        android:id="@+id/B3"
        android:layout_width="90dp"
        android:layout_height="wrap_content"
        android:background="#FFFF00"
        android:text="Yellow"
        app:layout_constraintRight_toRightOf="parent" />
    <Button
        android:id="@+id/B4"
        android:layout_width="60dp"
        android:layout_height="wrap_content"
        android:background="#0000FF"
        android:text="Blue"
        android:textColor="#FFFFFF"
        app:layout_constraintBottom_toTopOf="@+id/B7"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toBottomOf="@id/B2" />
    <Button
        android:id="@+id/B5"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_margin="10dp"
        android:background="#008000"
        android:text="GREEN"
        app:layout_constraintBaseline_toBaselineOf="@+id/B4"
        app:layout_constraintRight_toLeftOf="@+id/B4" />
    <Button
        android:id="@+id/B6"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_margin="10dp"
        android:background="#4B0082"
        android:text="Indigo"
        android:textColor="#FFFFFF"
        app:layout_constraintBaseline_toBaselineOf="@+id/B4"
        app:layout_constraintLeft_toRightOf="@+id/B4" />

    <Button
        android:id="@+id/B7"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:background="#EE82EE"
        android:text="Violet"
        app:layout_constraintBottom_toBottomOf="parent" />

</android.support.constraint.ConstraintLayout>
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190326104252743.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyMjQxNDEy,size_16,color_FFFFFF,t_70)
#### 3.利用表格布局实现如下：
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190326103643728.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyMjQxNDEy,size_16,color_FFFFFF,t_70)
<TableLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:stretchColumns=" * "
    android:background="#000000">
    <TableRow>
        <TextView
            android:layout_width="0dp"
            android:layout_weight="1"
            android:layout_height="wrap_content"
            android:layout_marginleft="10dp"
            android:text="Open..."
            android:background="#000000"
            android:textColor="#FFFFFF" />
        <TextView
            android:layout_width="0dp"
            android:layout_weight="1"
            android:layout_height="wrap_content"
            android:gravity="right"
            android:text="Crtl+O"
            android:textColor="#FFFFFF"/>
    </TableRow>
    <TableRow>
        <TextView
            android:layout_width="0dp"
            android:layout_weight="1"
            android:layout_height="wrap_content"
            android:layout_marginleft="10dp"
            android:text="Save..."
            android:background="#000000"
            android:textColor="#FFFFFF" />
        <TextView
            android:layout_width="0dp"
            android:layout_weight="1"
            android:layout_height="wrap_content"
            android:gravity="right"
            android:text="Crtl+S"
            android:textColor="#FFFFFF"/>
    </TableRow>
    <TableRow>
        <TextView
            android:layout_width="0dp"
            android:layout_weight="1"
            android:layout_height="wrap_content"
            android:layout_marginleft="10dp"
            android:text="Save as..."
            android:background="#000000"
            android:textColor="#FFFFFF" />
        <TextView
            android:layout_width="0dp"
            android:layout_weight="1"
            android:layout_height="wrap_content"
            android:gravity="right"
            android:text="Crtl=Shift+O"
            android:textColor="#FFFFFF"/>
    </TableRow>
    <view
        android:layout_width ="match_parent"
        android:layout_height ="2dp"
        android:background="#FFFFFF"/>
    <TableRow>
        <TextView
            android:layout_width="0dp"
            android:layout_weight="1"
            android:layout_height="wrap_content"
            android:layout_marginleft="10dp"
            android:text="X Import...."
            android:background="#000000"
            android:textColor="#FFFFFF" />
    </TableRow>
    <TableRow>
        <TextView
            android:layout_width="0dp"
            android:layout_weight="1"
            android:layout_height="wrap_content"
            android:layout_marginleft="10dp"
            android:text="X Export...."
            android:background="#000000"
            android:textColor="#FFFFFF" />
        <TextView
            android:layout_width="0dp"
            android:layout_weight="1"
            android:layout_height="wrap_content"
            android:gravity="right"
            android:text="Ctrl+E"
            android:textColor="#FFFFFF"/>
    </TableRow>
    <view
        android:layout_width ="match_parent"
        android:layout_height ="2dp"
        android:background="#FFFFFF"/>
    <TableRow>
        <TextView
            android:layout_width="0dp"
            android:layout_weight="1"
            android:layout_height="wrap_content"
            android:layout_marginleft="10dp"
            android:text="Quit"
            android:background="#000000"
            android:textColor="#FFFFFF" />
    </TableRow>
</TableLayout>
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190326104305834.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyMjQxNDEy,size_16,color_FFFFFF,t_70)
