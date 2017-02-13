## 循环结构 ##
循环：让程序*反复*执行同一段代码
 ***三要素:
    1. 循环条件：让循环*继续*执行的条件
 		比如: 圈数<3
    2. 循环变量：循环条件中用于比较的变量
                比如：圈数
            从几开始，(到几结束),每次变化几
            循环变量总要向着不满足循环条件的趋势不断变化
    3. 循环体：循环内，反复执行的代码段

    3种：
    1. while：先判断循环条件，再执行循环体
       何时使用：循环变量的变化，没有规律时
       语法：var 循环变量=初始值;
             while(循环条件){
             //当 
		循环体;
	 	迭代修改循环变量;
             }
```
var round=0;
     while(round<3){
      console.log("坐一圈");
      round++;
```

```
var input=-1;
     while((input=parseInt(prompt("请按键")))!=0){
      switch(input){
       case 1:
       console.log("查询中...");
       break;
       case 2:
       console.log("取款中...");
       break;
       case 3:
       console.log("转账进行中...");
       break;
       default:
       console.log("无效按键");
      }
     }
     console.log("欢迎下次光临！");
```

     2. do while: 先执行循环体，再判断循环条件
           何时使用：即使不满足循环条件，也希望至少执行一次时。
           语法：var 循环变量=初始值;
                 do{
    		循环体;
    	 	迭代修改循环变量;
                 }while(循环条件);
    
         while vs do while: 就看第一次条件是否满足
           第一次条件满足，两者完全等效
           第一次条件不满，while一次都不执行; do while至少可以执行一次.

