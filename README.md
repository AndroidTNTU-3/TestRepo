About
===
Drawing same shapes by a finger for building a flow chart.

## Getting Started

### 1. Reference in your XML like this.
```bash
<com.unrealedz.flowchartlib.DrawingView
        android:id="@+id/rlDrawView"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_alignParentLeft="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentTop="true" >
</com.unrealedz.flowchartlib.DrawingView>
```

### 2. Create helper classes.
```bash
//The shape`s manager 
ShapeManager shapeManager = new ShapeManager(getApplicationContext());
//Setting Api provide a base shape operations 
SettingsHelper settingsHelper = new SettingsHelper(getApplicationContext(), shapeManager);
//Drawing panel
DrawingView drawView = (DrawingView) findViewById(R.id.rlDrawView);
drawView.setShapeManager(shapeManager);
```

### 3. Integration.
```bash
dependencies {
    compile fileTree(include: ['*.jar'], dir: 'libs')
    compile 'com.android.support:appcompat-v7:22.2.1'
    compile project(':flowcahrtlib')
}
```


