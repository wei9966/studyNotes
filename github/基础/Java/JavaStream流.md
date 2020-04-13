## JavaStream流

[掘金JavaStream流](https://juejin.im/post/5e83fa28e51d4546d23bfd73)

#### Stream是什么

Stream 就好像一个高级的迭代器，但只能遍历一次，就好像一江春水向东流；在流的过程中，对流中的元素执行一些操作，比如“过滤掉长度大于 10 的字符串”、“获取每个字符串的首字母”等。

#### 实战

##### 创建流

1. 数组 Arrays.stream()或者Stream.of()创建流
2. 集合 
   1. 使用stream()方法创建流 
   2. 调用parallelStream() 默认使用的是ForkJoinPool.commponPool()线程池

##### 操作流程

1. 通过filter()方法可以筛选想要的元素
2. 使用map（）方法,把一个流中的元素转换成新的流中的元素
3. 匹配
   1. `anyMatch()`，只要有一个元素匹配传入的条件，就返回 true。`allMatch()`，只有有一个元素不匹配传入的条件，就返回 false；如果全部匹配，则返回 true。`noneMatch()`，只要有一个元素匹配传入的条件，就返回 false；如果全部匹配，则返回 true。

##### 转换流