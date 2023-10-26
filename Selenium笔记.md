# 这是新开的selenuim学习笔记

## selenium的底层原理

A:浏览器驱动、WebDriver接口、定位元素、执行JS、页面等待.

打开服务，占用端口，启动本地浏览器应用，WebDriver调用封装的Command类执行各种基于HTTP协议的指令.

## Selenium定位元素的方法

A：Selenium提供了多种方法来定位Web页面上的元素，以下是一些常用的元素定位方法：

1. 通过ID定位：
   使用`driver.findElement(By.id("elementId"))`方法，通过元素的唯一ID进行定位。

2. 通过Name定位：
   使用`driver.findElement(By.name("elementName"))`方法，通过元素的name属性进行定位。

3. 通过Class定位：
   使用`driver.findElement(By.className("className"))`方法，通过元素的class属性进行定位。

4. 通过Tag Name定位：
   使用`driver.findElement(By.tagName("tagName"))`方法，通过元素的标签名进行定位。

5. 通过XPath定位：
   使用`driver.findElement(By.xpath("xpathExpression"))`方法，通过XPath表达式进行定位。XPath提供了强大的灵活性，可以根据元素的层级关系、属性等进行定位。

6. 通过CSS选择器定位：
   使用`driver.findElement(By.cssSelector("cssSelector"))`方法，通过CSS选择器进行定位。CSS选择器提供了丰富的选择元素的方式，如类选择器、ID选择器、属性选择器等。

7. 通过Link Text定位：
   使用`driver.findElement(By.linkText("linkText"))`方法，通过链接文本进行定位。适用于定位`<a>`标签。

8. 通过Partial Link Text定位：
   使用`driver.findElement(By.partialLinkText("partialLinkText"))`方法，通过部分链接文本进行定位。适用于定位包含指定部分文本的`<a>`标签。

以上是一些常用的元素定位方法，根据具体的页面结构和需求，可以选择合适的方法来定位元素。如果定位到多个元素，可以使用`findElements()`方法获取元素列表，并进行进一步的操作。

## BUG定位

A:抓包工具验证传参内容；查看http请求参数和响应的结果；后端log日志有无错误信息；接口测试工具判断响应问题