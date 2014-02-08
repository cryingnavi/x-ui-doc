## X.View
x-ui의 가장 핵심이 되는 컴포넌트이다. X.View 는 대부분의 x-ui 컴포넌트의 상위 클래스이며 또한 컨테이너로서 다양한 html을 내포할 수 있다. 또한 X.View 들 간의 관계를 통해 다양한 레이아웃을 만들어 낼 수 있다.

[X.View](./assets/x-ui-1.0.3/doc/X.View.html)

```javascript
var view = new X.View({
	el: "#id",
	autoRender: true,
	content: "<!-- someting html -->"
});
```

```html
<div data-ui="view">
	<!-- someting html -->
</div>
```

