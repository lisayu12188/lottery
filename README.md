# lottery

抽奖功能的实现  

一.所用技术jQuery + CSS3过渡:transition,transform: rotate()  
二.基本思路：   
1. 将所有奖项保存到一个数组对象pool里；
2. 启动抽奖按钮后：  
  * s1.用box来保存剩余能抽的奖项；  
  * s2.预先随机获取box的下标，即随机产生一个奖项；  
  * s3.计算获取奖项在奖盘中的角度范围；（注意：计算必须要准确，最后指针指向的奖项才能和预先后台产生的奖项一致！）  
  * s4.奖盘随机旋转n圈+所取奖项的角度,奖盘停止转动所指向的奖项即为客户所中的奖项；  
