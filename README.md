记一些项目中遇到的第三方组件或框架，如果以下条目有更好的替代品，欢迎提出！Star and Respect All!

[GitHub Pages](https://cheatgz.github.io/Android-All-Star/)

- [界面](#界面)
  * [图片](#图片)
    + [android-gif-drawable](#android-gif-drawable)
    + [Glide](#glide)
    + [CircleImageView](#circleimageview)
    + [RoundedImageView](#roundedimageview)
    + [PhotoView](#photoview)
    + [subsampling-scale-image-view](#subsampling-scale-image-view)
    + [uCrop](#ucrop)
    + [PictureSelector](#pictureselector)
    + [Matisse](#matisse)
  * [文本](#文本)
    + [richeditor-android](#richeditor-android)
    + [TextSurface](#textsurface)
  * [弹窗](#弹窗)
    + [BaseDialog](#basedialog)
    + [material-dialogs](#material-dialogs)
    + [Toasty](#toasty)
  * [状态栏](#状态栏)
    + [ImmersionBar](#immersionbar)
    + [banner](#banner)
  * [指示器](#指示器)
    + [MagicIndicator](#magicindicator)
  * [图表](#图表)
    + [MPAndroidChart](#mpandroidchart)
    + [TableView](#tableview)
  * [角标](#角标)
    + [BGABadgeView-Android](#bgabadgeview-android)
  * [选择器](#选择器)
    + [Android-PickerView](#android-pickerview)
  * [欢迎页](#欢迎页)
    + [AppIntro](#appintro)
  * [菜单](#菜单)
    + [MaterialDrawer](#materialdrawer)
  * [日历](#日历)
    + [CalendarView](#calendarview)
  * [高斯模糊](#高斯模糊)
    + [blurkit-android](#blurkit-android)
  * [webview](#webview)
    + [AgentWeb](#agentweb)
  * [布局](#布局)
    + [vlayout](#vlayout)
    + [AndroidAutoSize](#androidautosize)
  * [其它](#其它)
    + [BaseRecyclerViewAdapterHelper](#baserecyclerviewadapterhelper)
    + [MultiLanguages](#multilanguages)
    + [QMUI_Android](#qmui_android)
    + [SmartRefreshLayout](#smartrefreshlayout)
  * [通信](#通信)
    + [ARouter](#arouter)
    + [EventBus](#eventbus)
    + [gson](#gson)
    + [retrofit)](#retrofit)
- [存储](#存储)
  + [[MMKV](#-mmkv--https---githubcom-tencent-mmkv-)
- [优化](#优化)
  + [leakcanary](#-leakcanary--https---githubcom-square-leakcanary-)
- [日志](#日志)
  + [logger](#-logger--https---githubcom-orhanobut-logger-)
  + [timber](#-timber--https---githubcom-jakewharton-timber-)
- [权限](#权限)
  + [PermissionX](#-permissionx--https---githubcom-guolindev-permissionx-)
- [不再推荐](#不再推荐)
  * [~~AndroidEventBus~~](#androideventbus)
  * [~~BadgeView~~](#badgeview)
  * [~~ButterKnife~~](#butterknife)
  * [~~CardSwipeLayout~~](#cardswipelayout)
  * [~~greenDAO~~](#greendao)
  * [~~MVPArms~~](#mvparms)
  * [~~NineOldAndroids~~](#nineoldandroids)
  * [~~NumberProgressBar~~](#numberprogressbar)
  * [~~picasso~~](#picasso)
  * [~~ViewPagerIndicator~~](#viewpagerindicator)

条目详细格式如下：

```
框架/组件       //框架或组件的Github地址，点击查看
GitHub 🌟：    //GitHub star星数
项目简介：      //框架或组件的简介
项目参考Blog：  //框架或组件可以参考如何使用的Blog
项目使用        //配置或添加框架、组件依赖
    implementation 'xx.xxx:xxx:x.x.x'
```

## 界面

### 图片

#### [android-gif-drawable](https://github.com/koral--/android-gif-drawable)

项目简介：Views and Drawable for displaying animated GIFs on Android

GitHub 🌟：8.7k

项目参考Blog：[android-gif-drawable教程](https://blog.csdn.net/feather_wch/article/details/79558240)

项目引入

```
    dependencies {
        ...
        implementation 'pl.droidsonroids.gif:android-gif-drawable:1.2.22'
    }
```

#### [Glide](https://github.com/bumptech/glide)

项目简介：An image loading and caching library for Android focused on smooth scrolling

GitHub 🌟：31k

项目参考Blog：[Glide使用总结](https://www.jianshu.com/p/791ee473a89b)

项目引入

```
      implementation 'com.github.bumptech.glide:glide:4.12.0'
      annotationProcessor 'com.github.bumptech.glide:compiler:4.12.0'
```

#### [CircleImageView](https://github.com/hdodenhof/CircleImageView)

项目简介：A fast circular ImageView perfect for profile images. 

GitHub 🌟：13.8k

项目参考Blog：[Android之CircleImageView使用(原创)](https://my.oschina.net/u/4410490/blog/3583355)

项目引入

```
    dependencies {
        ...
        implementation 'de.hdodenhof:circleimageview:3.1.0'
    }
```

#### [RoundedImageView](https://github.com/vinc3m1/RoundedImageView)

项目简介：A fast ImageView that supports rounded corners, ovals, and circles.

GitHub 🌟：6.2k

项目参考Blog：[Android 第三方RoundedImageView设置各种圆形、方形头像](https://blog.csdn.net/shenggaofei/article/details/83793536)

项目引入

```
    dependencies {
        ...
        implementation 'com.makeramen:roundedimageview:2.3.0'
    }
```

#### [PhotoView](https://github.com/chrisbanes/PhotoView)

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

#### [subsampling-scale-image-view](https://github.com/davemorrissey/subsampling-scale-image-view)

项目简介：Android library (AAR). Highly configurable, easily extendable deep zoom view for displaying huge images without loss of detail.

GitHub 🌟：6.7k

项目参考Blog：Subsampling Scale Image View [WiKi](https://github.com/davemorrissey/subsampling-scale-image-view/wiki/02.-Displaying-images)

项目引入

```
    dependencies {
        ...
        implementation 'com.davemorrissey.labs:subsampling-scale-image-view:3.10.0' // for support lib
        implementation 'com.davemorrissey.labs:subsampling-scale-image-view-androidx:3.10.0' // for androidx
    }
```

#### [uCrop](https://github.com/Yalantis/uCrop)

项目简介：Image Cropping Library for Android

GitHub 🌟：10.6k

项目参考Blog：[Android7.0拍照以及使用uCrop裁剪](https://juejin.cn/post/6844903495506591757)

项目引入

```
    dependencies {
        ...
        implementation 'com.github.yalantis:ucrop:2.2.6' //lightweight general solution
		implementation 'com.github.yalantis:ucrop:2.2.6-native' //get power of the native code to preserve image quality (+ about 1.5 MB to an apk size)
    }
```

#### [PictureSelector](https://github.com/LuckSiege/PictureSelector)

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


#### [Matisse](https://github.com/zhihu/Matisse)

项目简介：🎆 A well-designed local image and video selector for Android

GitHub 🌟：11.9k

项目参考Blog：[Matisse 知乎图片选择框架](https://www.jianshu.com/p/41e09238d61b)

项目引入

```
	repositories {
    	jcenter()
	}
	
    dependencies {
        ...
        implementation 'com.zhihu.android:matisse:$latest_version'
    }
```

### 文本

#### [richeditor-android](https://github.com/wasabeef/richeditor-android)

项目简介：RichEditor for Android is a beautiful Rich Text WYSIWYG Editor for Android.

GitHub 🌟：5.4k

项目参考Blog：[移动端强大的富文本编辑器richeditor-android](https://www.cnblogs.com/demodashi/p/10486780.html)

项目引入

```
	repositories {
  		mavenCentral()
	}

    dependencies {
        ...
        implementation 'jp.wasabeef:richeditor-android:2.0.0'
    }
```

#### [TextSurface](https://github.com/elevenetc/TextSurface)

项目简介：A little animation framework which could help you to show message in a nice looking way

GitHub 🌟：2.1k

项目参考Blog：[一个Android文字展示动画框架：TextSurface](https://www.open-open.com/lib/view/open1446797002013.html)

项目引入

```
	repositories {
    	maven { url "https://jitpack.io" }
	}
    dependencies {
        ...
        implementation 'com.github.elevenetc:textsurface:0.9.1'
    }
```
### 弹窗

#### [BaseDialog](https://github.com/AnJiaoDe/BaseDialog)

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

#### [material-dialogs](https://github.com/afollestad/material-dialogs)

项目简介：😍 A beautiful, fluid, and extensible dialogs API for Kotlin & Android.

GitHub 🌟：18.7k

项目参考Blog：[material-dialogs/documentation](https://github.com/afollestad/material-dialogs/tree/main/documentation)

项目引入

```
    dependencies {
        ...
        implementation 'com.afollestad.material-dialogs:core:3.3.0'
    }
```

#### [Toasty](https://github.com/GrenderG/Toasty)

项目简介：The usual Toast, but with steroids 💪

GitHub 🌟：6.1k

项目参考Blog：[Usage](https://github.com/GrenderG/Toasty#usage)

项目引入

```
    dependencies {
        ...
        implementation 'com.github.GrenderG:Toasty:1.5.0'
    }
```

### 状态栏

#### [ImmersionBar](https://github.com/gyf-dev/ImmersionBar)

项目简介：Android 4.4以上沉浸式状态栏和沉浸式导航栏管理

GitHub 🌟：9.5k

项目参考Blog：[android4.4以上沉浸式状态栏和导航栏实现以及Bar的其他管理](https://www.jianshu.com/p/2a884e211a62)

项目引入

```
    dependencies {
        ...
        // 基础依赖包，必须要依赖
		implementation 'com.gyf.immersionbar:immersionbar:3.0.0'
		// fragment快速实现（可选）
		implementation 'com.gyf.immersionbar:immersionbar-components:3.0.0'
		// kotlin扩展（可选）
		implementation 'com.gyf.immersionbar:immersionbar-ktx:3.0.0'
    }
```

### 轮播图

#### [banner](https://github.com/youth5201314/banner)

项目简介：只做一个可以自定义的轮播容器，不侵入UI ———— Banner 2.0

GitHub 🌟：11.1k

项目参考Blog：[Banner2.0 GitHub介绍](https://github.com/youth5201314/banner)

项目引入

```
    implementation 'com.youth.banner:banner:2.1.0'
```

### 指示器

#### [MagicIndicator](https://github.com/hackware1993/MagicIndicator)

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
### 图表

#### [MPAndroidChart](https://github.com/PhilJay/MPAndroidChart)

项目简介：A powerful 🚀 Android chart view / graph view library, supporting line- bar- pie- radar- bubble- and candlestick charts as well as scaling, panning and animations.

GitHub 🌟：33.1k

项目参考Blog：[detailed video tutorials(付费视频)](https://weeklycoding.com/downloads/)、[MPAndroidChart Documentation](https://weeklycoding.com/mpandroidchart-documentation/)

项目引入

```
    repositories {
        ...
        maven {
            url "https://jitpack.io"
        }
    }

    dependencies {
    	implementation 'com.github.PhilJay:MPAndroidChart:v3.1.0'
    }
```

#### [TableView](https://github.com/evrencoskun/TableView)

项目简介：TableView is a powerful Android library for displaying complex data structures and rendering tabular data composed of rows, columns and cells

GitHub 🌟：2.8k

项目参考Blog：[Welcome to the Documentation of the TableView library](https://github.com/evrencoskun/TableView/wiki)

项目引入

```
	dependencies {
    	implementation 'com.evrencoskun.library:tableview:0.8.9.4'
	}
```

### 角标

#### [BGABadgeView-Android](https://github.com/bingoogolapple/BGABadgeView-Android)

项目简介：Android 徽章控件

GitHub 🌟：2.4k

项目参考Blog：[初始化徽章控件](https://github.com/bingoogolapple/BGABadgeView-Android#初始化徽章控件)

项目引入

```
	//把 maven { url 'https://jitpack.io' } 加入到 repositories 中
	repositories {
    	maven { url "https://jitpack.io" }
	}
	
    dependencies {
        ...
        implementation 'com.github.bingoogolapple.BGABadgeView-Android:api:latestVersion'
    	annotationProcessor 'com.github.bingoogolapple.BGABadgeView-Android:compiler:latestVersion'
    }
```

### 选择器

#### [Android-PickerView](https://github.com/Bigkoo/Android-PickerView)

项目简介：This is a picker view for android , support linkage effect, timepicker and optionspicker.（时间选择器、省市区三级联动）

GitHub 🌟：12.7k

项目参考Blog：[PickerView--仿ios滚轮时间选择、城市选择效果](https://blog.csdn.net/wangwo1991/article/details/85036891)

项目引入

```
    implementation 'com.contrarywind:Android-PickerView:4.1.9'
```

### 欢迎页

#### [AppIntro](https://github.com/AppIntro/AppIntro)

项目简介：Make a cool intro for your Android app.

GitHub 🌟：9.7k

项目参考Blog：[Basic usage](https://github.com/AppIntro/AppIntro#basic-usage)

项目引入

```
	repositories {
    	maven { url "https://jitpack.io" }
	}

    dependencies {
        ...
        implementation 'com.github.AppIntro:AppIntro:4.2.3' // for support lib
        implementation 'com.github.AppIntro:AppIntro:6.1.0' // for androidx
    }
```

### 菜单

#### [MaterialDrawer](https://github.com/mikepenz/MaterialDrawer)

项目简介：The flexible, easy to use, all in one drawer library for your Android project. Now brand new with material 2 design

GitHub 🌟：11.3k

项目参考Blog：[Android, Using Navigation Drawer Across Multiple Activities: The easiest way.](https://medium.com/android-news/android-using-navigation-drawer-across-multiple-activities-the-easiest-way-b011f152aebd)

项目引入

```
    implementation "com.mikepenz:materialdrawer:${lastestMaterialDrawerRelease}"

	//required support lib modules
	implementation "androidx.appcompat:appcompat:${versions.appcompat}"
	implementation "androidx.recyclerview:recyclerview:${versions.recyclerView}"
	implementation "androidx.annotation:annotation:${versions.annotation}"
	implementation "com.google.android.material:material:${versions.material}"
	implementation "androidx.constraintlayout:constraintlayout:${versions.constraintLayout}"

	// Add for NavController support
	implementation "com.mikepenz:materialdrawer-nav:${lastestMaterialDrawerRelease}"

	// Add for Android-Iconics support
	implementation "com.mikepenz:materialdrawer-iconics:${lastestMaterialDrawerRelease}"
```

### 日历

#### [CalendarView](https://github.com/huanghaibin-dev/CalendarView)

项目简介：Android上一个优雅、万能自定义UI、支持周视图、自定义周起始、性能高效的日历控件，支持热插拔实现的UI定制！

GitHub 🌟：7.5k

项目参考Blog：[CalendarView使用详细文档](https://github.com/huanghaibin-dev/CalendarView/blob/master/QUESTION_ZH.md)

项目引入

```
    dependencies {
        ...
        implementation 'com.haibin:calendarview:3.6.8' // for support lib
        implementation 'com.haibin:calendarview:3.7.1' // for androidx
    }
```

### 高斯模糊

#### [blurkit-android](https://github.com/CameraKit/blurkit-android)

项目简介：Android上一个优雅、万能自定义UI、支持周视图、自定义周起始、性能高效的日历控件，支持热插拔实现的UI定制！

GitHub 🌟：3.4k

项目参考Blog：[Usage](https://github.com/CameraKit/blurkit-android#usage)

项目引入

```
    dependencies {
        ...
        implementation 'io.alterac.blurkit:blurkit:1.1.0'
    }
```

### webview

#### [AgentWeb](https://github.com/Justson/AgentWeb)

项目简介：AgentWeb is a powerful library based on Android WebView.

GitHub 🌟：8k

项目参考Blog：[WebView 性能和用户体验优化](https://www.jianshu.com/p/fc7909e24178)

项目引入

```
    dependencies {
        ...
        implementation 'com.just.agentweb:agentweb:4.1.4' // (必选)
		implementation 'com.just.agentweb:filechooser:4.1.4'// (可选)
		implementation 'com.download.library:Downloader:4.1.4'// (可选) // for support lib
		
        implementation 'com.just.agentweb:agentweb-androidx:4.1.4' // (必选)
		implementation 'com.just.agentweb:filechooser-androidx:4.1.4'// (可选)
		implementation 'com.download.library:downloader-androidx:4.1.4'// (可选) // for androidx
    }
```

### 布局

####  [vlayout](https://github.com/alibaba/vlayout)

项目简介：Project vlayout is a powerfull LayoutManager extension for RecyclerView, it provides a group of layouts for RecyclerView. Make it able to handle a complicate situation when grid, list and other layouts in the same recyclerview.

GitHub 🌟：10.7k

项目参考Blog：[vlayout--让你的多布局不再头疼](https://www.jianshu.com/p/5fb06a52a12d)

项目引入

```
    implementation ('com.alibaba.android:vlayout:1.2.8@aar') {
	    transitive = true
    }
```

#### [AndroidAutoSize](https://github.com/JessYanCoding/AndroidAutoSize)

项目简介：🔥 A low-cost Android screen adaptation solution (今日头条屏幕适配方案终极版，一个极低成本的 Android 屏幕适配方案).

GitHub 🌟：11.3k

项目参考Blog：[今日头条屏幕适配方案终极版，一个极低成本的 Android 屏幕适配方案.](https://github.com/JessYanCoding/AndroidAutoSize/blob/master/README-zh.md)

项目引入

```
    dependencies {
        ...
        implementation 'me.jessyan:autosize:1.2.1'
    }
```

### 其它 

#### [BaseRecyclerViewAdapterHelper](https://github.com/CymChad/BaseRecyclerViewAdapterHelper)

项目简介：BRVAH:Powerful and flexible RecyclerAdapter

GitHub 🌟：21.7k

项目参考Blog：[BRVAH官网](http://www.recyclerview.org/)

项目引入

```
    implementation 'com.github.CymChad:BaseRecyclerViewAdapterHelper:3.0.4'
```

#### [MultiLanguages](https://github.com/MichaelJokAr/MultiLanguages)

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

#### [QMUI_Android](https://github.com/Tencent/QMUI_Android)

项目简介：提高 Android UI 开发效率的 UI 库

GitHub 🌟：12.8k

项目参考Blog：QMUI_Android[官网](https://qmuiteam.com/android)

项目引入

```
	//最新的库会上传到 JCenter 仓库上，请确保配置了 JCenter 仓库源
    dependencies {
        ...
        implementation 'com.qmuiteam:qmui:2.0.0-alpha10'
    }
```

#### [SmartRefreshLayout](https://github.com/scwang90/SmartRefreshLayout)

项目简介：🔥下拉刷新、上拉加载、二级刷新、淘宝二楼、RefreshLayout、OverScroll，Android智能下拉刷新框架，支持越界回弹、越界拖动，具有极强的扩展性，集成了几十种炫酷的Header和 Footer

GitHub 🌟：22.4k

项目参考Blog：[Android智能下拉刷新框架-SmartRefreshLayout](https://segmentfault.com/a/1190000010066071)

项目引入

如果使用 AndroidX 先在 gradle.properties 中添加，两行都不能少噢~

```
    android.useAndroidX=true
    android.enableJetifier=true
```

需要依赖 androidx.appcompat

```
    implementation 'androidx.appcompat:appcompat:1.0.0'                 //必须 1.0.0 以上

    implementation  'com.scwang.smart:refresh-layout-kernel:2.0.3'      //核心必须依赖
    implementation  'com.scwang.smart:refresh-header-classics:2.0.3'    //经典刷新头
    implementation  'com.scwang.smart:refresh-header-radar:2.0.3'       //雷达刷新头
    implementation  'com.scwang.smart:refresh-header-falsify:2.0.3'     //虚拟刷新头
    implementation  'com.scwang.smart:refresh-header-material:2.0.3'    //谷歌刷新头
    implementation  'com.scwang.smart:refresh-header-two-level:2.0.3'   //二级刷新头
    implementation  'com.scwang.smart:refresh-footer-ball:2.0.3'        //球脉冲加载
    implementation  'com.scwang.smart:refresh-footer-classics:2.0.3'    //经典加载
```

### 通信

#### [ARouter](https://github.com/alibaba/ARouter)

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

#### [EventBus](https://github.com/greenrobot/EventBus)

项目简介：Event bus for Android and Java that simplifies communication between Activities, Fragments, Threads, Services, etc. Less code, better quality

GitHub 🌟：23.3k

项目参考Blog：[Android EventBus 的使用](https://www.jianshu.com/p/e7d5c7bda783)

项目引入

```
  implementation 'org.greenrobot:eventbus:3.2.0'
```

#### [gson](https://github.com/google/gson)

项目简介：A Java serialization/deserialization library to convert Java Objects into JSON and back

GitHub 🌟：19.4k

项目参考Blog：[GSON](https://www.jianshu.com/p/75a50aa0cad1)

项目引入

```
    implementation 'com.google.code.gson:gson:2.8.6'
```

#### [retrofit](https://github.com/square/retrofit)

项目简介：A type-safe HTTP client for Android and Java.

GitHub 🌟：37.9k

项目参考Blog：[Retrofit官网](https://square.github.io/retrofit/)

项目引入

```
    implementation 'com.squareup.retrofit2:retrofit:(insert latest version)'
```

## 存储

#### [MMKV](https://github.com/Tencent/MMKV)

项目简介：MMKV 是基于 mmap 内存映射的 key-value 组件，底层序列化/反序列化使用 protobuf 实现，性能高，稳定性强，可以替代SharedPreferences

GitHub 🌟：12.4k

项目参考Blog：[MMKV——1.使用](https://www.jianshu.com/p/bc6d8b714635)、[MMKV——2.原理](https://www.jianshu.com/p/83ee82c30e53)

项目引入

```
       implementation 'com.tencent:mmkv-static:1.2.7'
       // replace "1.2.7" with any available version
```

## 优化

#### [leakcanary](https://github.com/square/leakcanary)

项目简介：A memory leak detection library for Android

GitHub 🌟：25.9k

项目参考Blog：[LeakCanary官网](https://square.github.io/leakcanary/)

项目引入

```
      // debugImplementation because LeakCanary should only run in debug builds.
      debugImplementation 'com.squareup.leakcanary:leakcanary-android:2.7'
```

## 日志

#### [logger](https://github.com/orhanobut/logger)

项目简介：Simple, pretty and powerful logger for android

GitHub 🌟：12.1k

项目参考Blog：[Android 日志记录杂谈-Logger,Timber,logback-android](https://www.jianshu.com/p/39834be3cb6c)

项目引入

```
  implementation 'com.orhanobut:logger:2.2.0'
```

#### [timber](https://github.com/JakeWharton/timber)

项目简介：A logger with a small, extensible API which provides utility on top of Android's normal Log class.

GitHub 🌟：8.8k

项目参考Blog：1.[Timber: Android日志记录](https://www.jianshu.com/p/4f54fcba3ad3) 2.[Android 日志记录杂谈-Logger,Timber,logback-android](https://www.jianshu.com/p/39834be3cb6c)

项目引入

```
  implementation 'com.jakewharton.timber:timber:4.7.1'
```

## 权限

#### [PermissionX](https://github.com/guolindev/PermissionX)

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
