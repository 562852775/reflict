reflict
=======

how to user reflict

String className = "com.kaishengit.entity.Car"; 
//根据类名创建类的对象 
Object obj = Class.forName(className).newInstance();
//获取对象的Class对象 
Class clazz = obj.getClass(); 
//获取所有的方法 
Method[] methods = clazz.getMethods(); 
//获取指定方法 
Method method = clazz.getMethod("start"); 
//执行方法 
method.invoke(obj); 
 
