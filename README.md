记一些项目中遇到的第三方组件或框架，如果以下条目有更好的替代品，欢迎提出！Star and Respect All!

[GitHub Pages](https://cheatgz.github.io/Android-All-Star/)

## 目录
- [UI](#ui)
  * [Android-PickerView](#android-pickerview)
  * [banner](#banner)
  * [BaseDialog](#basedialog)
  * [BaseRecyclerViewAdapterHelper](#baserecyclerviewadapterhelper)
  * [MagicIndicator](#magicindicator)
  * [MultiLanguages](#multilanguages)
  * [PhotoView](#photoview)
  * [PictureSelector](#pictureselector)
  * [RoundedImageView](#roundedimageview)
  * [vlayout](#vlayout)
- [通信](#通信)
  * [ARouter](#arouter)
  * [EventBus](#eventbus)
  * [gson](#gson)
  * [retrofit](#retrofit)
- [图片](#图片)
  * [Glide](#glide)
- [存储](#存储)
  * [MMKV](#mmkv)
- [优化](#优化)
  * [leakcanary](#leakcanary)
- [日志](#日志)
  * [logger](#logger)
  * [timber](#timber)
- [权限](#权限)
  * [PermissionX](#permissionx)
- [不再推荐](#不再推荐)
  * ~~[AndroidEventBus](#androideventbus)~~
  * ~~[BadgeView](#badgeview)~~
  * ~~[ButterKnife](#butterknife)~~
  * ~~[CardSwipeLayout](#cardswipelayout)~~
  * ~~[greenDAO](#greendao)~~
  * ~~[MVPArms](#mvparms)~~
  * ~~[NineOldAndroids](#nineoldandroids)~~
  * ~~[NumberProgressBar](#numberprogressbar)~~
  * ~~[picasso](#picasso)~~
  * ~~[ViewPagerIndicator](#viewpagerindicator)~~

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>

条目详细格式如下：

```
框架/组件       //框架或组件的Github地址，点击查看
GitHub 🌟：    //GitHub star星数
项目简介：      //框架或组件的简介
项目参考Blog：  //框架或组件可以参考如何使用的Blog
项目使用        //配置或添加框架、组件依赖
    implementation 'xx.xxx:xxx:x.x.x'
```

## UI

### [Android-PickerView](https://github.com/Bigkoo/Android-PickerView)

项目简介：This is a picker view for android , support linkage effect, timepicker and optionspicker.（时间选择器、省市区三级联动）

GitHub 🌟：12.7k

项目参考Blog：[PickerView--仿ios滚轮时间选择、城市选择效果](https://blog.csdn.net/wangwo1991/article/details/85036891)

项目引入

```
    implementation 'com.contrarywind:Android-PickerView:4.1.9'
```

### [banner](https://github.com/youth5201314/banner)

项目简介：只做一个可以自定义的轮播容器，不侵入UI ———— Banner 2.0

GitHub 🌟：11.1k

项目参考Blog：[Banner2.0 GitHub介绍](https://github.com/youth5201314/banner)

项目引入

```
    implementation 'com.youth.banner:banner:2.1.0'
```

### [BaseDialog](https://github.com/AnJiaoDe/BaseDialog)

项目简介：Android BaseDialog(开发必备)动画、加载进度、阴影、上下左右中 进入

GitHub 🌟：163

项目参考Blog：[Android BaseDialog(开发必备)动画、加载进度、阴影](https://blog.csdn.net/confusing_awakening/article/details/78332459)

项目引入

```
    implementation 'com.github.AnJiaoDe:BaseDialog:V1.1.8'
```

```
    allprojects {
       repositories {
          jcenter()
          maven { url 'https://jitpack.io' }
       }
    }
```

### [BaseRecyclerViewAdapterHelper](https://github.com/CymChad/BaseRecyclerViewAdapterHelper)

项目简介：BRVAH:Powerful and flexible RecyclerAdapter

GitHub 🌟：21.7k

项目参考Blog：[BRVAH官网](http://www.recyclerview.org/)

项目引入

```
    implementation 'com.github.CymChad:BaseRecyclerViewAdapterHelper:3.0.4'
```

### [MagicIndicator](https://github.com/hackware1993/MagicIndicator)

项目简介：强大、可定制、易扩展的 ViewPager 指示器框架。是ViewPagerIndicator、TabLayout、PagerSlidingTabStrip的最佳替代品

GitHub 🌟：8.6k

项目参考Blog：[MagicIndicator系列之一 —— 使用MagicIndicator打造千变万化的ViewPager指示器](https://www.jianshu.com/p/2865812fed41)

项目引入

```
    repositories {
        ...
        maven {
            url "https://jitpack.io"
        }
    }

    dependencies {
        ...
        implementation 'com.github.hackware1993:MagicIndicator:1.6.0' // for support lib
        implementation 'com.github.hackware1993:MagicIndicator:1.7.0' // for androidx
    }
```

### [MultiLanguages](https://github.com/MichaelJokAr/MultiLanguages)

项目简介：Android 多语言切换（兼容8.0+） 2.0版本，一句代码完成多语言切换，现在支持第三方包里多语言切换（前提是有对应的语言资源）

GitHub 🌟：300

项目参考Blog：[MultiLanguages/README_cn.md](https://github.com/MichaelJokAr/MultiLanguages/blob/master/README_cn.md)

项目引入

在APP的build.gradle文件下引入gradle plugin

```
    buildscript {
        dependencies {
            classpath 'com.github.jokar:multi-languages.plugin:<latest-version>'
        }
    }
```

在模块的build.gradle文件中引入plugin

```
    apply plugin: 'multi-languages'
    ...
    android{
        defaultConfig { 
            multiLanguages {
                //set plugin is enable( default)
                enable = true
            }
        }
    }
    ...
    dependencies {
        implementation 'com.github.jokar:multi-languages:<latest-version>'
    }
    
```

### [PhotoView](https://github.com/chrisbanes/PhotoView)

项目简介：Implementation of ImageView for Android that supports zooming, by various touch gestures.

GitHub 🌟：17.6k

项目参考Blog：[Android UI Libs之PhotoView](https://www.jianshu.com/p/680f4859a000)

项目引入

```
    implementation 'com.github.chrisbanes:PhotoView:latest.release.here'
```

Add this in your root build.gradle file (not your module build.gradle file):

```
    allprojects {
       repositories {
          jcenter()
          maven { url 'https://jitpack.io' }
       }
    }
    buildscript {
        repositories {
          maven { url "https://www.jitpack.io" }
       }	
    }
```

### [PictureSelector](https://github.com/LuckSiege/PictureSelector)

项目简介：Picture Selector Library for Android or 多图片选择器

GitHub 🌟：10.1k

项目参考Blog：[Android 选择图片、上传图片之PictureSelector](https://blog.csdn.net/yechaoa/article/details/79291552)

项目引入

```
    implementation 'com.github.LuckSiege.PictureSelector:picture_library:v2.6.0'
```

```
    allprojects {
       repositories {
          jcenter()
          maven { url 'https://jitpack.io' }
       }
    }
```

### [RoundedImageView](https://github.com/vinc3m1/RoundedImageView)

项目简介：A fast ImageView that supports rounded corners, ovals, and circles.

GitHub 🌟：6.2k

项目参考Blog：[Android 第三方RoundedImageView设置各种圆形、方形头像](https://blog.csdn.net/shenggaofei/article/details/83793536)

项目引入

```
    implementation 'com.makeramen:roundedimageview:2.3.0'
```

###  [vlayout](https://github.com/alibaba/vlayout)

项目简介：Project vlayout is a powerfull LayoutManager extension for RecyclerView, it provides a group of layouts for RecyclerView. Make it able to handle a complicate situation when grid, list and other layouts in the same recyclerview.

GitHub 🌟：10.7k

项目参考Blog：[vlayout--让你的多布局不再头疼](https://www.jianshu.com/p/5fb06a52a12d)

项目引入

```
    implementation ('com.alibaba.android:vlayout:1.2.8@aar') {
	    transitive = true
    }
```

## 通信

### [ARouter](https://github.com/alibaba/ARouter)

项目简介：一个用于帮助 Android App 进行组件化改造的框架 —— 支持模块间的路由、通信、解耦

GitHub 🌟：13k

项目参考Blog：[ARouter/README_CN.md](https://github.com/alibaba/ARouter/blob/master/README_CN.md)

项目引入

```
    android {
        defaultConfig {
            ...
            javaCompileOptions {
                annotationProcessorOptions {
                    arguments = [AROUTER_MODULE_NAME: project.getName()]
                }
            }
        }
    }

    dependencies {
        // 替换成最新版本, 需要注意的是api
        // 要与compiler匹配使用，均使用最新版可以保证兼容
        compile 'com.alibaba:arouter-api:x.x.x'
        annotationProcessor 'com.alibaba:arouter-compiler:x.x.x'
        ...
    }
    // 旧版本gradle插件(< 2.2)，可以使用apt插件，配置方法见文末'其他#4'
    // Kotlin配置参考文末'其他#5'
```

### [EventBus](https://github.com/greenrobot/EventBus)

项目简介：Event bus for Android and Java that simplifies communication between Activities, Fragments, Threads, Services, etc. Less code, better quality

GitHub 🌟：23.3k

项目参考Blog：[Android EventBus 的使用](https://www.jianshu.com/p/e7d5c7bda783)

项目引入

```
  implementation 'org.greenrobot:eventbus:3.2.0'
```

### [gson](https://github.com/google/gson)

项目简介：A Java serialization/deserialization library to convert Java Objects into JSON and back

GitHub 🌟：19.4k

项目参考Blog：[GSON](https://www.jianshu.com/p/75a50aa0cad1)

项目引入

```
    implementation 'com.google.code.gson:gson:2.8.6'
```

### [retrofit](https://github.com/square/retrofit)

项目简介：A type-safe HTTP client for Android and Java.

GitHub 🌟：37.9k

项目参考Blog：[Retrofit官网](https://square.github.io/retrofit/)

项目引入

```
    implementation 'com.squareup.retrofit2:retrofit:(insert latest version)'
```

## 图片

### [Glide](https://github.com/bumptech/glide)

项目简介：An image loading and caching library for Android focused on smooth scrolling

GitHub 🌟：31k

项目参考Blog：[Glide使用总结](https://www.jianshu.com/p/791ee473a89b)

项目引入

```
      implementation 'com.github.bumptech.glide:glide:4.12.0'
      annotationProcessor 'com.github.bumptech.glide:compiler:4.12.0'
```

## 存储

### [MMKV](https://github.com/Tencent/MMKV)

项目简介：MMKV 是基于 mmap 内存映射的 key-value 组件，底层序列化/反序列化使用 protobuf 实现，性能高，稳定性强，可以替代SharedPreferences

GitHub 🌟：12.4k

项目参考Blog：[MMKV——1.使用](https://www.jianshu.com/p/bc6d8b714635)、[MMKV——2.原理](https://www.jianshu.com/p/83ee82c30e53)

项目引入

```
       implementation 'com.tencent:mmkv-static:1.2.7'
       // replace "1.2.7" with any available version
```

## 优化

### [leakcanary](https://github.com/square/leakcanary)

项目简介：A memory leak detection library for Android

GitHub 🌟：25.9k

项目参考Blog：[LeakCanary官网](https://square.github.io/leakcanary/)

项目引入

```
      // debugImplementation because LeakCanary should only run in debug builds.
      debugImplementation 'com.squareup.leakcanary:leakcanary-android:2.7'
```

## 日志

### [logger](https://github.com/orhanobut/logger)

项目简介：Simple, pretty and powerful logger for android

GitHub 🌟：12.1k

项目参考Blog：[Android 日志记录杂谈-Logger,Timber,logback-android](https://www.jianshu.com/p/39834be3cb6c)

项目引入

```
  implementation 'com.orhanobut:logger:2.2.0'
```

### [timber](https://github.com/JakeWharton/timber)

项目简介：A logger with a small, extensible API which provides utility on top of Android's normal Log class.

GitHub 🌟：8.8k

项目参考Blog：1.[Timber: Android日志记录](https://www.jianshu.com/p/4f54fcba3ad3) 2.[Android 日志记录杂谈-Logger,Timber,logback-android](https://www.jianshu.com/p/39834be3cb6c)

项目引入

```
  implementation 'com.jakewharton.timber:timber:4.7.1'
```

## 权限

### [PermissionX](https://github.com/guolindev/PermissionX)

项目简介：PermissionX is an extension Android library that makes Android runtime permission request extremely easy

GitHub 🌟：1.6k

项目参考Blog：[PermissionX-作者:guolin](https://blog.csdn.net/guolin_blog/category_10108528.html)

项目引入

```
  implementation 'com.permissionx.guolindev:permissionx:1.4.0'
```

## 不再推荐

以下条目是因**GitHub更新时间过久**、**已停止维护**、**有更好替代品**等原因被推荐替换的项目

**GitHub更新时间过久**：GitHub上次更新时间过久，作者可能已经放弃维护，使用时可能会产生BUG，请谨慎考虑使用

**已停止维护**：作者已明确声明项目停止维护，不再提供功能更新、BUG修复，不推荐使用此类项目

**有更好替代品**：此类项目仍然推荐使用，但有更好的开源框架或者官方库可以替代

条目详细格式如下：

```
框架/组件           //框架或组件的Github地址，点击查看
GitHub 🌟：        //GitHub star星数
GitHub更新时间      //GitHub上次更新时间
Releases最新版本：  //GitHub上最新的Releases版本
不再推荐原因：         //因某种原因，推荐使用其它框架或组件替换
替代框架：          //推荐使用的替代框架或组件
```

###  ~~[AndroidEventBus](https://github.com/hehonghui/AndroidEventBus)~~

GitHub 🌟：1.6k

GitHub更新时间：2018年3月

Releases最新版本：2015年5月 Version-1.0.4

不推荐原因：已停止维护[DEPRECATED] 

替代框架：无

###  ~~[BadgeView](https://github.com/qstumn/BadgeView)~~

GitHub 🌟：3.9k

GitHub更新时间：2017年4月

Releases最新版本：2017年9月 Version-1.1.3

不推荐原因：已停止维护[DEPRECATED]

替代框架：无

### ~~[ButterKnife](https://github.com/JakeWharton/butterknife)~~

GitHub 🌟：25.7k

GitHub更新时间：2020年9月

Releases最新版本：2020年8月 Version-10.2.3

不推荐原因：已停止维护[DEPRECATED] 

替代框架：官方JetPack库的[DataBinding](https://developer.android.google.cn/jetpack/androidx/releases/databinding?hl=zh-cn)、官方的[ViewBinding](https://developer.android.google.cn/topic/libraries/view-binding?hl=zh-cn)

###  ~~[CardSwipeLayout](https://github.com/yuqirong/CardSwipeLayout)~~

GitHub 🌟：1.1k

GitHub更新时间：2017年3月

Releases最新版本：无Release版本

不推荐原因：GitHub更新时间过久

替代框架：无

### ~~[greenDAO](https://github.com/greenrobot/greenDAO)~~

GitHub 🌟：12.4k

GitHub更新时间：2021年2月

Releases最新版本：2020年5月 Version-3.3.0

不推荐原因：使用比较复杂，有更好替代品

替代框架：官方JetPack库的[Room](https://developer.android.google.cn/jetpack/androidx/releases/room?hl=zh-cn)、郭霖大神的[LitPal](https://github.com/guolindev/LitePal)

### ~~[MVPArms](https://github.com/JessYanCoding/MVPArms/wiki#1)~~

GitHub 🌟：10k

GitHub更新时间：2020年6月

Releases最新版本：2019年7月 Version-2.5.2

不推荐原因：有更好的替代品

替代框架：官方推荐的MVVM架构，配合JetPack可以很轻松搭建MVVM架构，使用[官方JetPack库](https://developer.android.google.cn/jetpack?hl=zh-cn)搭建MVVM架构

###  ~~[NineOldAndroids](https://github.com/JakeWharton/NineOldAndroids)~~

GitHub 🌟：4.5k

GitHub更新时间：2014年10月

Releases最新版本：2012年6月 Version-2.4.0

不推荐原因：已停止维护[DEPRECATED] 

替代框架：无

###  ~~[NumberProgressBar](https://github.com/daimajia/NumberProgressBar)~~

GitHub 🌟：5.9k

GitHub更新时间：2017年7月

Releases最新版本：2014年8月 Version-1.2

不推荐原因：GitHub更新时间过久

替代框架：无

###  ~~[picasso](https://github.com/square/picasso)~~

GitHub 🌟：17.9k

GitHub更新时间：2020年9月

Releases最新版本：2020年8月 Version-2.8

不推荐原因：有更好的替代品

替代框架：[Glide](https://github.com/bumptech/glide)

###  ~~[ViewPagerIndicator](https://github.com/LinweiJ/ViewPagerIndicator)~~

GitHub 🌟：368

GitHub更新时间：2019年8月

Releases最新版本：2019年8月 Version-0.3.0

不推荐原因：有更好的替代品

替代框架：[MagicIndicator](https://github.com/hackware1993/MagicIndicator)https://github.com/hackware1993/MagicIndicator)
