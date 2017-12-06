# NestRadioGroup
可嵌套ViewGroup&amp;View的自定义RadioGroup


# Pic

示意图



![image](https://github.com/RealMoMo/NestRadioGroup/blob/master/pic/show1.jpg)

![image](https://github.com/RealMoMo/NestRadioGroup/blob/master/pic/shoew2.jpg)


## 属性介绍

name               | format      |中文解释
----               |------       |----
vertical           | boolean   	 |布局方向是否垂直


<br/>

## xml布局代码
```
<FrameLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context="com.hht.nestradiogrouptest.MainActivity">

    <com.hht.view.NestRadioGroup
        android:id="@+id/group"
        app:vertical="true"
        android:layout_width="match_parent"
        android:layout_height="match_parent">

       
            <RelativeLayout
                android:id="@+id/layout1"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content">

                <RadioButton

                    android:layout_margin="10dp"
                    android:id="@+id/rb1"
                    android:text="111111"
                    android:layout_width="100dp"
                    android:layout_height="100dp" />

                <ImageView
                    android:id="@+id/iv1"
                    android:layout_marginLeft="100dp"
                    android:src="@drawable/check"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content" />


            </RelativeLayout>


          、、、


            <ImageView
                android:layout_alignTop="@+id/layout1"
                android:layout_toRightOf="@+id/layout1"
                android:id="@+id/iv"
                android:src="@drawable/source"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content" />


            <RelativeLayout
                android:layout_marginLeft="150dp"
                android:layout_below="@+id/iv"
                android:id="@+id/layout4"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content">

                <RadioButton
                    android:layout_margin="10dp"
                    android:id="@+id/rb4"
                    android:layout_width="100dp"
                    android:layout_height="100dp"
                    android:text="44444" />

                <ImageView
                    android:id="@+id/iv4"
                    android:layout_marginLeft="100dp"
                    android:src="@drawable/check"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content" />


            </RelativeLayout>


           、、、

        </RelativeLayout>



    </com.hht.view.NestRadioGroup>

</FrameLayout>

```
<br/>


## Thanks
	Everyone who has contributed code and reported issues and pull requests!


## License

	Licensed under the Apache License, Version 2.0 (the "License");
	you may not use this file except in compliance with the License.
	You may obtain a copy of the License at

	   http://www.apache.org/licenses/LICENSE-2.0

	Unless required by applicable law or agreed to in writing, software
	distributed under the License is distributed on an "AS IS" BASIS,
	WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
	See the License for the specific language governing permissions and
	limitations under the License.