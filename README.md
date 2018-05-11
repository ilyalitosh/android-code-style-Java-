# Android code convention

### Content
1. [Comments/javadoc](#comments_javadoc)<br>
2. [Short methods](#short_methods)<br>
3. [Methods name](#methods_name)<br>
4. [Fields](#fields)<br>
5. [Local variables](#local_variables)<br>
6. [Imports](#imports)<br>
7. [Indents](#indents)<br>
8. [String length](#string_length)<br>
9. [Braces](#braces)<br>
10. [Reductions](#reductions)<br>
11. [TODO and FIXME](#TODO_and_FIXME)<br>
12. [Consistency](#consistency)<br>
13. [Resources files](#resources_files)<br>
14. [Android components classes](#android_components_classes)<br>
15. [Packages](#packages)<br>
16. [Project package](#project_package)<br>
17. [Package structure](#package_structure)<br>

<a name="comments_javadoc"><h2>Comments/javadoc</h2></a>

    Each class and public method must contain Javadoc, with at least one phrase describing what it does.
<br>    For example:
<br> 
```java
public interface DbBaseModel {

    /**
     * Returns String with insert result
     * @param rows insert string count
     */
    String insertingResult(int rows);

}
```

<a name="short_methods"><h2>Short methods</h2></a>

    Methods should be small and decisives specific tasks, as far as possible.
<br>    For example:
```java
public class RealmService implements IEntityGenerator<Car>{  
  
    @Override  
    public Car generateEntity(long id) {  
        Car car = new Car();  
        car.setColor("Black");  
        car.setFuelCapacity(113);  
        car.setPrice(666);  
        car.setId(id);  
  
        return car;  
    }  
  
} 
```

<a name="methods_name"><h2>Methods name</h2></a>

    The method names must be verbs written according to the CamelCase principle. Method names should not contain abbreviations, unless these abbreviations are abbreviations or acronyms.
<br>    For example:
```java
// YES 
@Override  
public String insertingResult(int rows) {  
    return null;  
}  
// NO
@Override  
public String insertingRes(int rows) {  
    return null;  
} 
```

<a name="fields"><h2>Fields</h2></a>

    The fields must be at the top of the file, or right before the method that uses them. 
<br>    Private non-static fields must begin with the letter ```m```. 
<br>    Private and static fields must begin with the letter ```s```.
<br>    All names of fields, classes, methods should be written according to the principle of CamelCase.
<br>    Constant field is writing with uppercase and with ```_```.
    For example:
```java
public class HomeActivity extends MvpAppCompatActivity{  
  
    private AppCompatSpinner mSpinnerDB;  
    private AppCompatSpinner mSpinnerType;  
    private TextView mDbResultView;  
    private Button mSubmitButton;  
    private EditText mInputRows;  
    private EditText mInputId;  
    public static final int CONSTANT_NUMBER = 5;  
    DBResultPresenter mDbResultPresenter;  
    private static Singlton sSinglton;  
  
} 
```

<a name="local_variables"><h2>Local variables</h2></a>

    The scope of local variables must be kept to a minimum. Each variable must be declared in the deepest block that surrounds all possible places of use of the variable.
<br>Local variables must be declared in the place, where it is first necessary to use it.
<br>For example: 
![1](resources/local_variables_screen.png)<br>

<a name="imports"><h2>Imports</h2></a>

The ordering of import statements is:
<br>    1. Android imports.
<br>    2. Imports from third parties (com, junit, net, org).
<br>    3. java and javax packages.
<br>Imports must be:
<br>    - Alphabetical within each grouping.
<br>    - Capital letters before lower case letters (e.g. Z before a).
<br>    - Separated by a blank line between each major grouping.
<br>For example: 
```java
import android.os.Bundle;  
import android.support.v7.widget.AppCompatSpinner;  
import android.text.TextUtils;  
import android.widget.ArrayAdapter;  
import android.widget.Button;  
import android.widget.EditText;  
import android.widget.TextView;  
import android.widget.Toast;  
  
import com.arellomobile.mvp.MvpAppCompatActivity;  
import com.arellomobile.mvp.presenter.InjectPresenter;  
import com.ilya.litosh.roomvsrealm.R;  
import com.ilya.litosh.roomvsrealm.presenters.DBChooserPresenter;  
import com.ilya.litosh.roomvsrealm.presenters.DBResultPresenter;  
import com.ilya.litosh.roomvsrealm.presenters.TypeChooserPresenter;  
import com.ilya.litosh.roomvsrealm.views.DBChooserView;  
import com.ilya.litosh.roomvsrealm.views.DBResultView;  
import com.ilya.litosh.roomvsrealm.views.TypeChooserView;  
  
import java.util.List; 
```

<a name="Indents"><h2>Indents</h2></a>



<a name="string_length"><h2>String length</h2></a>

<a name="braces"><h2>Braces</h2></a>

<a name="reductions"><h2>Reductions</h2></a>

<a name="TODO_and_FIXME"><h2>TODO and FIXME</h2></a>

<a name="consistency"><h2>Consistency</h2></a>

<a name="resources_files"><h2>Resources files</h2></a>

<a name="android_components_classes"><h2>Android components classes</h2></a>

<a name="packages"><h2>Packages</h2></a>

<a name="project_package"><h2>Project package</h2></a>

<a name="package_structure"><h2>Package structure</h2></a>




