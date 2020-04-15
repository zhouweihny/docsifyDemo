## 快速导航

- [mk语法](#mk语法)

## mk语法
```markdown
# 一级标题

## 二级标题

### 三级标题

#### 四级标题
```

- 一个段落只能有一个主题，或一个中心句子。
- 段落的中心句子放在段首，对全段内容进行概述。后面陈述的句子为核心句服务。
- 一个段落的长度不能超过七行，最佳段落长度小于等于四行。
- 段落的句子语气要使用陈述和肯定语气，避免使用感叹语气。
- 段落之间使用一个空行隔开。
- 段落开头不要留出空白字符。


> 词法作用域由写代码期间函数所声明的位置来定义，javascript有两种机制(eval()、with)在运行时来修改词法作用域，这样做通常会导致性能下降，内存泄漏问题。

* ```JavaScript```七种内置类型: ```number、string、boolean、undefined、null、object、symbol```(ES6新增加)
* ```基本类型：```指保存在栈内存中的数据，```引用类型：```([对象引用]())指保存在堆内存中的对象，传递的是引用的地址
* ```弱类型：```变量没有类型, 变量持有的值有类型
* ```(typeof null === 'object') = true```，正确的返回值应该是```null```，但是这个```bug```由来已久。 ```(undefined == null) = true```
* ```indexOf```为```ECMAScript5```新方法，```IE8```及以下不支持
-  ```setTimeout(callback, 100)```，```setTimeout```只接受一个函数或者变量做为参数不接受闭包，因为闭包会自执行，最小延迟```4ms```

```js
{
function withObj(obj){
	with(obj){
		a = 2
	}
}

let o1 = {
	a: 1,
}

let o2 = {
	b: 1,
}

withObj(o1);
console.log(o1.a); // 2

withObj(o2);
console.log(o2.a); // undefined
console.log(a); // 2
}
```

```
引用One man’s constant is another man’s variable. — Alan Perlis
```
------

## 感谢

[《Node.js技术栈》](https://www.nodejs.red/#/)

[《中文技术文档的写作规范》](https://github.com/ruanyf/document-style-guide/blob/master/README.md)

[《Cmd Markdown 编辑阅读器》](https://www.zybuluo.com/mdeditor)

