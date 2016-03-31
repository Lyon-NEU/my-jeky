---
layout: post
title: "LinkedList"
description: ""
category: 
tags: [Java]
---
{% include JB/setup %}



## 常用方法

* `getFirst()`,`getLast()`获取列表第一个、最后一个元素
* `addFirst()`与`add()`和`addLast()`相同，都将某个元素插入到列表的尾(端)部。

```Java

public class LinkedListTest {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		LinkedList<String> list=new LinkedList<String>();
		list.add("1");  
		list.add("2");  
		list.add("3");  
		list.add("4");  
		list.add("5");  
		list.add("6");
	  	list.addFirst("0");
	  	list.addLast("7");
	    System.out.println("链表的第一个元素是 : " + list.getFirst());  
	    System.out.println("链表最后一个元素是 : " + list.getLast()); 
	}
}

//output: 
链表的第一个元素是 : 0
链表最后一个元素是 : 7
```

* LinkedList也像ArrayList一样实现了List的接口，但是在执行某些操作(中间的插入、删除)时比ArrayList更高效，但在随机访问操作方面要逊色一些。

* LikedList添加了可以使其用作栈、队列或双端队列的方法

* removeFirst()与remove()功能一样，它们移除并返回列表的头，在列表为空时抛出NoSuchElementException,poll()在列表为空时返回null，removeLast()移除并返回列表的最后一个元素。
