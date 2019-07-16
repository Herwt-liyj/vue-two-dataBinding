# vue-two-dataBinding
vue的双向数据绑定mock
### 3、对象的定义
#### Object.defineProperty(obj, prop, descriptor)
参数：
    obj：必要的目标对象
    prop：必要的需要定义或者修改的属性名
    descriptor：必要的目标属性全部拥有的属性
返回值：
返回传入的第一个参数；即第一个参数obj

    Object.defineProperty(obj,'name',{
    	configurable:true,   //控制是否可删除
    	enumerable:true,    //控制是否可以枚举
    	writable:true,      //控制是否可以修改赋值
    	value:'任意类型的值,默认undefined'
	})
	
	注意：当 writable:true, configurable:false 时 enumerable默认false,
	如下：
	Object.defineProperty(obj2,'idkey',{
    	configurable:false,
    	writable:true,
    	value:'idkey'
    })
    总结：Object.defineProperty()给对象添加属性；如果不设置属性的特性；则默认值都为false， Object.defineProperty(obj,'name',{})，
    configurable:是否可删除， writable:是否可修改赋值， enumerable:是否可枚举
    
### 4、vue的双向数据绑定
参考链接地址：https://segmentfault.com/a/1190000014423018

参考文章：https://segmentfault.com/a/1190000014423018
