![82e607796f00b8058866ba07ede2dc68.png](en-resource://database/569:1)
![8f7f66259a918c775b83e982e9370572.png](en-resource://database/571:1)

- 变量名之前\*号，接收>=1 个变量，封装为元组，接收到空就是空元组

元组拆包，\*变量名, 会是将剩余装到列表中
``` python
students = {'01':('赵铁柱',20,222), '02':('诸葛钢铁',21), '03':('王钢蛋',21)}   # 字典 key = value
def print_boy(name, **person):    
    if isinstance(person, dict):      # isinstance(object, calssinfo) 输出布尔类型        
		values = person.values()        
		print(values)        
		for name, *age in person.values():           
			print('{}的年龄是{}'.format(name,age))

```

将字典拆包， \*\*变量名，则是将剩余装到元组中