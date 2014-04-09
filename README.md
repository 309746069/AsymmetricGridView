# AsymmetricGridView

An Android listView that implements multiple columns and variable sized elements.

Still very very unstable!

### Usage

```xml
<com.felipecsl.asymmetricgridview.library.widget.AsymmetricGridView
    xmlns:android="http://schemas.android.com/apk/res/android"
    android:id="@+id/listView"
    android:layout_width="match_parent"
    android:layout_height="match_parent"/>
```

```java
@Override
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_main);
    listView = (AsymmetricGridView) findViewById(R.id.listView);
    // Choose your own preferred column width
    listView.setRequestedColumnWidth(Utils.dpToPx(this, 120));
    final List<AsymmetricItem> items = new ArrayList<>();
    // initialize your items array
    adapter = new ListAdapter(this, listView, items);
    listView.setAdapter(adapter);
}
```

### [Demo Youtube video](https://www.youtube.com/watch?v=hVmk3wUpbaY&feature=youtu.be)

### Screenshots:

![](https://raw.githubusercontent.com/felipecsl/AsymmetricGridView/master/screenshots/ss_2_cols.png)
![](https://raw.githubusercontent.com/felipecsl/AsymmetricGridView/master/screenshots/ss_3_cols.png)
![](https://raw.githubusercontent.com/felipecsl/AsymmetricGridView/master/screenshots/ss_4_cols.png)
![](https://raw.githubusercontent.com/felipecsl/AsymmetricGridView/master/screenshots/ss_5_cols.png)

### Contributing

* Check out the latest master to make sure the feature hasn't been implemented or the bug hasn't been fixed yet
* Check out the issue tracker to make sure someone already hasn't requested it and/or contributed it
* Fork the project
* Start a feature/bugfix branch
* Commit and push until you are happy with your contribution
* Make sure to add tests for it. This is important so I don't break it in a future version unintentionally.

### Copyright and license

Code and documentation copyright 2011-2014 Felipe Lima.
Code released under the [MIT license](https://github.com/felipecsl/AsymmetricGridview/blob/master/LICENSE.txt).