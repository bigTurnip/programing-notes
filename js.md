# 内存数据

1. number
2. string
3. boolean
4. undefined
5. null
6. symbol
7. object
   1. 函数
   2. class
   3. ArrayBuffer

所谓传递就是变量与变量之间的赋值。字面量是一种匿名变量。前6种属于值传递，第7种属于址传递。

前6种数据类型在运行时会转换成对应的包装对象。

# 数据类型的用法

1. symbol

```js
const value=Symbol('key') // 创建一个symbol
const value2=Symbol.for('key') // 从作用域获取一个symbol
const key=Symbol.keyFor(value) //获取一个symbol的key，key=='key'
```

2. array

```plain
数组切片
Array.slice(start,end)

去除数组元素,并插入
Array.splice(start,len,ele...)

映射，返回内容组成新数组
Array.map((item,index)=>{})

遍历数组
Array.forEach((item,index)=>{})

过滤数组，返回为true的组成新数组
Array.filter((item,index)=>{})

查找数组，有一个返回true就为true
Array.some((item,index)=>{})

查找数组，全部返回true就为true
Array.every((item,index)=>{})

Arr to String
Arr.join(',')
```

3. string

```plain
切片
String.slice(start,end)
String.substr(start,end)
String.substring(start,end)

String to Arr
String,split(',')
```

# 流程控制

1. 顺序控制

```plain
程序是从上到下依次执行
```

2. 分支控制

```js
// if控制
if(cond){}
else if(cond){}
else{}

// switch控制
switch(cond){
    case '1':
        break;
    case '2':
        break;
    default:
        break;
}
```

2. 循环控制

```js
// break表示跳出当前全部循环，continue表示跳出当前本次循环
break
continue

// label标记。break，continue默认跳出本循环，使用label后可以跳出指定循环
let num = 0;
outPoint:
for (var i = 0 ; i < 10 ; i++){
  for (var j = 0 ; j < 10 ; j++){
    if( i == 5 && j == 5 ){
      break outPoint
    }
    num++
  }
}
alert(num); // 输出 55

// for循环
for(let i=0;i<len;i++){}

// while循环
while(cond){}

// do while语句
do{

}while(cond)

// for in遍历数组和对象，值是对象的属性值或数组元素
for(const value in Arr){

}

// for of遍历数组和对象，值是属性名或数组下标
for(const value of Arr){

}
```