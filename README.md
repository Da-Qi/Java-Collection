# Java-Collection
学习集合模块札记

# Collection🔘
## List😀
### ArrayList😁
底层数据结构为数组，查询快，增删慢，线程不安全，效率高。
### Vector😁
底层数据结构为数组，查询快，增删慢，线程安全，效率低。
### LinkedList😁
底层数据结构为链表，查询慢，增删快，线程不安全，效率高。

## Set😀
### HashSet😊
不保证Set的迭代顺序，具备唯一性，在存储自定义对象时重写hashcode()、equals()方法;
底层数据结构为哈希表（元素是链表的数组），哈希表依赖于哈希值存储。
#### LinkedHashSet
底层数据结构为 哈希表 和 链表 组成。保证了唯一性和有序性。
### TreeSet😊
底层为二叉树，因此具有排序和唯一性；
无参构造时，默认为自然数排序
其排序可分为：

a.自然排序：实现接口Comparable，重写方法，设置先后条件；

b.比较器排序：实现接口Comparator，通过匿名内部类或者重写实现；


## 集合的遍历
A. 增强for

B. 迭代器排序

Iterator it = 集合.iterator();   调用 hasNext()、next()方法实现遍历
