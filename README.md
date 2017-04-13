# 高仿IOS时间选择器


引用 <br>  
allprojects {<br>  
    repositories {<br>  
        jcenter()<br>  
        maven { url "https://jitpack.io" }<br>  
    }<br>  
}<br>  
compile 'com.github.guyueyang:timePicket:5.0'<br>  
<br>  
创建对象 <br>
 private TimePickerShow timePickerShow;<br>  
 timePickerShow=new TimePickerShow(this);<br>  
 <br>  
 监听放回值<br>
   timePickerShow.setOnTimePickerListener(new TimePickerShow.OnTimePickerListener() {<br>  
            @Override<br>  
            public void onClicklistener(String dataTime) {<br>  
                Toast.makeText(getApplicationContext(),dataTime,Toast.LENGTH_LONG).show();<br>  
            }<br>  
        });<br>  
        <br>  
 显示<br>
 timePickerShow.timePickerAlertDialog("1991-01-01");<br>
 传入时间格式"yyyy-MM-dd"  可以为空   空 默认为当前时间<br>  

