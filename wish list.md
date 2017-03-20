## wish list

###  知识点

1.`localStorage`

> HTML5 提供了两种在客户端存储数据的新方法：
>
> - localStorage - 没有时间限制的数据存储（localStorage 方法存储的数据没有时间限制。第二天、第二周或下一年之后，数据依然可用。）
> - sessionStorage - 针对一个 session 的数据存储（sessionStorage 方法针对一个 session 进行数据存储。当用户关闭浏览器窗口后，数据会被删除。）

- `localStorage.setItem(key, value)`:存储数据
- `locaStorage.getItem(key)`:从strorage中读取数据

2.`JSON.stringfy()`：解析一个JSON字符串，构造由字符串描述的JavaScript值或对象。

3.`JSON.parse()`:从字符串中解析出JSON对象

4.`template strings`:模板字符串。模板字符串使用反引号来代替普通字符串中的用双引号和单引号。模板字符串可以包含特定语法`${expression}` 。相较于传统的字符串拼接的方式，使用模板字符串真的可以省时省力不少。

e.g

```javascript
`
<li>
  <input type="checkbox" data-index=${i}  id="item${i}" 	${wish.done ? 'checked':''} />
  <label for="${i}">${wish.text}
	<span class="hide">${'x'}</span>
  </label>
</li>
`
```

6.`label`

> for 属性规定 label 与哪个表单元素绑定。

label标签的for属性值是为了对应其相应的input元素的id，只有进行对应时，才能进行选择。如果不做对应，点击标签时，不能进行选择。

## 主要功能

1.读取localstorage中存储的数据，在页面上渲染出来。

2.添加新的list,存储数据。

- 获取填写的内容

  `const text = document.querySelector('[name=item]').value`

- 将获取的数据，已经完成的状态存储为以对象的形式存储到一个数组里。

3.标记列表项完成情况，存储数据。





















