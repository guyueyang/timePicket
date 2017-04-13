# 高仿IOS时间选择器


#1引用 /<br>  
allprojects {
    repositories {
        jcenter()
        maven { url "https://jitpack.io" }
    }
}
compile 'com.github.guyueyang:timePicket:5.0'

#1 创建对象 /<br>
 private TimePickerShow timePickerShow;
 timePickerShow=new TimePickerShow(this);
 
 #1 监听放回值/<br>
   timePickerShow.setOnTimePickerListener(new TimePickerShow.OnTimePickerListener() {
            @Override
            public void onClicklistener(String dataTime) {
                Toast.makeText(getApplicationContext(),dataTime,Toast.LENGTH_LONG).show();
            }
        });
        
 #1 显示/<br>
 timePickerShow.timePickerAlertDialog("1991-01-01");/<br>
 传入时间格式"yyyy-MM-dd"  可以为空   空 默认为当前时间

