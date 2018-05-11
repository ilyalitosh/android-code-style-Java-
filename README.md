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
<br>For example:
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
<br>For example:
```java
public class RealmService IEntityGenerator<Car>{  
  
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

<a name="fields"><h2>Fields</h2></a>

<a name="local_variables"><h2>Local variables</h2></a>

<a name="imports"><h2>Imports</h2></a>

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




