# `<z-panel>`

Panel element which has header to toggle content display

## Attributes

- `primary`: primary panel style
- `static`: could not be collapsed
- `collapsed`: collapsed by default

## Methods

- `toggle()`
- `close()`
- `open()`

## Example

```
<style>z-panel {max-width: 640px; margin-bottom: 2em;}</style>

<p><z-btn id="z-panel-toggle">toggle!</z-btn></p>

<z-panel id="z-panel-test">
  <header>HEADER</header>
  CONTENT
</z-panel>

<z-panel primary collapsed>
  <header>HEADER COLLAPSED BY DEFAULT</header>
  CONTENT
</z-panel>

<z-panel static>
  <header>STATIC HEADER</header>
  CONTENT
</z-panel>

<z-panel>
  PANEL CONTENT WITHOUT HEADER
</z-panel>

<script>
  var btn = document.querySelector('html /deep/ #z-panel-toggle');
  var panel = document.querySelector('html /deep/ #z-panel-test');

  btn.addEventListener('click', function (e) {
    panel.toggle();
  });
</script>
```
