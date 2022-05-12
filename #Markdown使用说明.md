# Markdown使用说明
## 一、标题
使用`#`表示标题，写在行首不能缩进，从#到######分别表示一号到六号标题（依次缩小）
**<font color=blue> 例如：</font>**
# `#` 一号标题
## `##` 二号标题 
### `###` 三号标题 
#### `####` 四号标题
##### `#####` 五号标题 
###### `######` 六号标题 
## 二、分割线
使用三个或以上的 -(下划线) 或者 * 表示，且这一行只有符号，<br/>注意不要被识别为二级标题即可，例如中间或者前面可以加空格。
**例如：**
___
***
## 三、粗体、斜体、删除线
使用`*`表示斜体，`**`表示粗体，`~~`表示删除线
例如：
*我是斜体*  
**我是粗体** 
***我是又粗又斜*** 
~~我是已删除的文字~~
## 四、超链接和图片
超链接: `[显示文字]（url）` 
或者 `[显示文字][1]  `
     ` [1]:url`
图片的显示方法是再查链接的前面加个`！`
例如：
[Markdown 语法](https://blog.csdn.net/afei__/article/details/80717153)<br/>
[百度百科Markdown](https://baike.baidu.com/item/markdown/3245829?fr=aladdin)<br/>
![Markdown Log](https://bkimg.cdn.bcebos.com/pic/d009b3de9c82d158ccbf98bc1b430ed8bc3eb135e42e?x-bce-process=image/resize,m_lfit,w_440,limit_1/format,f_auto)

## 五、无序列表 和 有序列表

## 六、代码块 和 行内代码块
```CSharp
        private object[,] getEditRangeValue()
        {
            object[,] arr = editRange.Value;
            for (int i = 1; i <= arr.Length; i++)
            {
                if (arr[1, i] == null)
                    arr[1, i] = "";
            }
            return arr;
        }
```
```sql
select staffNo from View_staffinfo where realName=''
```
## 七、表格

## 八、流程图

```flow
st=>start: 用户登录
e=>end: 结束
op1=>inputoutput: 输入用户名和密码
sub1=>subroutine: 用户名或密码错误
cond=>condition: 验证通过?
io=>operation: 写登录日志

st->op1->cond
cond(yes)->io->e
cond(no)->sub1(right)->op1
```

## 九、数学公式

## 十、支持HTML标签