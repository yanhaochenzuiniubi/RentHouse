# 基于用户性格模型的线上租房平台
**1.模块架构**
_此项目是基于B/S架构，使用Java EE开发，框架使用SpringBoot2.2版本，整个网站的系统主要模式是使用了MVC架构模式_。


**2.算法实现**
_此算法根据欧式距离来进行设计，欧式距离的相似度是最常见的距离度量，衡量的是多维空间中两个点之间的绝对距离_。


理论公式为：![捕获](https://user-images.githubusercontent.com/70590957/180751080-2fc3a610-4ff7-45d2-965c-3f312b91a279.PNG)




_程序实现如下：_
'''public double euclidean (double []x,double []y ){
int length  = x.length;
 double sum = 0;
for (int i = 0; i < length; i++){
            sum= Math.pow((x[i] - y[i]),2) +sum;
        }
        return Math.sqrt(sum);
    }
}'''
_系统将用户所填性格量表的数据转换成数组，将两名用户的性格数据作为函数的输入，通过调用上述程序，计算两用户间的欧式距离并输出_。
