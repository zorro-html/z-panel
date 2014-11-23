# panel

面板

* 可折叠
* 有默认和 `[primary]` 2 种内置样式
* 可以通过 `static` 特性/属性禁用折叠效果 (永远展开)
* 可以通过 `collapsed` 特性/属性确定折叠状态
* 可以通过 `toggle()`, `close()`, `open()` 方法控制折叠动作

## 特性&属性

### `static`

禁用折叠效果 (永远展开)

### `collapsed`

标识内容是否已折叠起来

### `toggle()`, `close()`, `open()`

切换/折叠/展开

## Example

```
<p><jie-btn>toggle!</jie-btn></p>

<jie-panel>
  <header>HEADER</header>
  CONTENT
</jie-panel>

<jie-panel primary collapsed>
  <header>HEADER</header>
  CONTENT
</jie-panel>

<jie-panel static>
  CONTENT
</jie-panel>

<script>
  var btn = document.querySelector('jie-btn');
  var panel = document.querySelector('jie-panel');

  btn.addEventListener('click', function (e) {
    panel.toggle();
  });
</script>
```
