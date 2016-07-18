# note-for-Android-koma
My note for the tourist of Android

# 全屏显示的方式
1.<!--去掉标题栏--> 
 <style name="Theme.AppCompat.Light.NoActionBar">
    <item name="windowActionBar">false</item>
    <item name="windowNoTitle">true</item>
</style>
<!--全屏属性-->
<item name="android:windowFullscreen">true</item>
2. #在java代码中实现全屏(必须在setContentView之前调用)
requestWindowFeature(Window.FEATURE_NO_TITLE); //无title  
getWindow().setFlags(WindowManager.LayoutParams.FLAG_FULLSCREEN,WindowManager.LayoutParams.FLAG_FULLSCREEN); //全屏  

#在代码中禁用StatusBar的方法
 //hide statusbar 
	StatusBarManager sbm = (StatusBarManager) this.getSystemService("statusbar");    
	sbm.disable(StatusBarManager.DISABLE_MASK);
 //display StatusBar 
	StatusBarManager sbm = (StatusBarManager) this.getSystemService("statusbar");    
	sbm.disable(StatusBarManager.DISABLE_NONE);
	
	#

