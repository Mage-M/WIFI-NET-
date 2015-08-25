# WIFI-NET-
这里总结了一些android设备对wifi状态，wifiAP状态，手机网络状态获取及判别的使用方法总结


WIFIAP的状态获取：
1.当android设备的WIFIAP打开或者关闭时，系统会主动发出一条全局广播android.net.wifi.WIFI_AP_STATE_CHANGED


2.我们可以自定义一个广播接收器，用来监听系统发出的这条广播，当收到广播时，我们就可以获取WIFIAP现在的状态
 
 
  ->WIFIAP有四种状态：（1） WIFI_STATE_DISABLED                     
                       (2)  WIFI_STATE_DISABLING
                       (3)  WIFI_STATE_ENABLED
                       (4)  WIFI_STATE_ENABLING
