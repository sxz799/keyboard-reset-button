# KeyBoardResetForMac
通过修改注册表修正三模键盘在mac模式下对win系统的兼容性

## 开发背景
因为现在常见的三模键盘虽然提供了mac模式,但是mac模式的按键映射是全局的，并没有绑定到某一模式
我最终想实现的效果如下
```
使用蓝牙模式连接mac
使用有线模式连接pc
```
在切换模式后可自行实现键盘映射 
但是没有键盘固件源码，毕竟这个需求只是个人需要所以就换个思路实现
即 键盘一直处在mac模式下，去修改windows系统的按键映射实现想要的效果
所以现在只实现了左右 ctrl alt win 按键的映射，有更多的需求可以直接修改keyMap/keyMap.go 添加即可

