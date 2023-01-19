# Page 1

Чтобы анимировать svg нужно получить длину path:

```javascript
const svgPath = document.querySelector('svg path');
const pathLength = svgPath.getTotalLength();
```

Дальше можем присвоить это значение в css-переменную:

```javascript
svgPath.style.setProperty('--path-length', pathLength);
```

Анимировать будем изменяя значение `stroke-dashoffset` от `var(--path-length)` до `0`.

```css
svg path {
  stroke-dasharray: var(--path-length);
  stroke-dashoffset: var(--path-length);
  animation: pathAnimation 10s linear forwards;
}

@keyframes pathAnimation {
  to {
    stroke-dashoffset: 0;
  }
}
```
