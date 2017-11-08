# LooperRecView
一个匀速循环展示item的小项目
# 展示效果
![img](https://github.com/YRInred/LooperRecView/blob/master/01074.gif)
# 添加依赖
```compile
compile 'com.github.YRInred:LooperRecView:1.0'
```
# 使用方法
## 在xml文件中添加
```xml
    <com.inred.looperrecview.NoScrollRecyclerView
        android:id="@+id/noscroll_rec"
        android:layout_centerInParent="true"
        android:layout_width="match_parent"
        android:paddingTop="10dp"
        android:paddingBottom="10dp"
        android:layout_height="140dp"
        android:background="@color/white"
        android:orientation="vertical"
        app:speed="20"/>
```
## 在java文件中添加
```java
 noscroll_rec = findViewById(R.id.noscroll_rec);
        LooperAdapter adapter = new LooperAdapter(getList());
        noscroll_rec.setAdapter(adapter);
```
注意LooperAdapter 必须继承 LooprecAdapter
目前这个recyclerview不能手动滑动 不用添加manager 只能改变滑动速度 后期会增加
