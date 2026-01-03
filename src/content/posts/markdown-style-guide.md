---
title: 'Markdown 样式指南'
pubDate: '2025-06-28'
---

本主题未定义更多级别的标题，如有需要，可在 `src/styles/post.css` 文件中自行定义。

---

## 段落

下面是 Markdown 段落的实际示例。这段文字演示了博客文章中内容的自然流动。

你可以在段落中使用多种格式选项，比如 **加粗**、_斜体_、~~删除线~~ 以及 `代码`。

## 引用块

> 不要通过共享内存进行交流，而应通过交流来共享内存。<br>
> — <cite>Rob Pike[^1]</cite>

[^1]: 上述引语摘自 Rob Pike 于 2015 年 11 月 18 日 Gopherfest 的[演讲](https://www.youtube.com/watch?v=PAAkCSZUG1c)。

### 有序列表

1. 第一项
2. 第二项
3. 第三项

### 无序列表

- 项目
  - 子项
  - 子项

## 任务列表

- [ ] 第一项
- [ ] 第二项
- [x] 第三项

## 图片

如果要隐藏图片说明，请用下划线 `_` 开头，或留空 alt 文本。

![HIKARI](./_assets/hikari.jpg)

## 表格

| 样式   | 粗细     | 其它   |
| ------ | -------- | ------ |
| 常规   | 常规     | 文字   |
| _斜体_ | **粗体** | `代码` |

## 代码块

```jsx
// Button.jsx

const Button = ({ text, onClick }) => {
  const [count, setCount] = useState(0)

  const handleClick = () => {
    setCount(count + 1)
    onClick?.()
  }

  return (
    <button className="btn" onClick={handleClick}>
      {text} ({count})
    </button>
  )
}
```

## 其他元素 — sub, sup, abbr, kbd, mark

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

<abbr title="Graphics Interchange Format">GIF</abbr> 是一种位图图像格式。

按下 <kbd>CTRL</kbd> + <kbd>ALT</kbd> + <kbd>Delete</kbd> 可结束会话。

大多数 <mark>蝾螈</mark> 是夜行性的，以昆虫、蠕虫及其它小型生物为食。

---
