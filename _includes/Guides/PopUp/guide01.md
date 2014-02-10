## [팝업](#popup)
팝업은 X.View 의 floating 프로퍼티를 true 로 설정함으로써 간단히 생성할 수 있다. 


[X.View](./assets/x-ui-1.0.3/doc/X.View.html)

```javascript
var view = new X.View({
	el: "#id",
	autoRender: true,
	content: "<!-- someting html -->",
	floating: true
});

//show
view.show();

//hide
view.hide();
```

```html
<div data-ui="view" data-floating="true" style="width: 300px;height:300px;" id="popup">
	<!-- someting html -->
</div>


X..util.cm.get("popup").show();
//hide
X..util.cm.get("popup")..hide();
```

