# panel

面板

* 可折叠
* 有默认和 `[primary]` 2 种内置样式
* 可以通过 `[collapsed]` 特性、`collapsed` 属性、`toggle()`, `close()`, `open()` 方法控制折叠状态

## 特性&属性

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

<jie-panel>
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
