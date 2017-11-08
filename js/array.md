#JS array
[TOC]
###稀疏数组与密集数组
    稀疏数组：数组元素的索引不连续
```//稀疏数组
 var array = new Array(3);
 array[2] = "name";
 for(var a in array)
 {
    console.log("index=" + a + ",value=" + array[a]);
 }
 // 密集数组
 var dense = Array.apply(null, Array(3));
 dense[2] = "name";
 for(var a in dense)
 {
    console.log("index=" + a + ",value=" + dense[a]);
 }```
