---
layout: page
title : Guide
header : Post Archive
group: navigation
---
{% include JB/setup %}


## Application 생성하기
```javascript
X.App({
	ready: function(){
		//application init
	}
});
```


## X.View
x-ui의 가장 핵심이 되는 컴포넌트이다. X.View 는 컨테이너이며 다양한 html을 내포할 수 있다. 또한 X.View 들 간의 관계를 통해 다양한 레이아웃을 만들어 낼 수 있다.
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

## 레이아웃 만들기
```html
<!-- header -->
<div data-ui="view" data-flexible="false" style="height: 100px;">
	<!-- someting html -->
</div>

<!-- body -->
<div data-ui="view">
	<!-- someting html -->
</div>
```



```html
<div data-ui="view" data-layout="x">
	<!-- left -->
	<div data-ui="view" data-flexible="false" style="width: 100px;">
		<!-- someting html -->
	</div>

	<!-- body -->
	<div data-ui="view">
		<!-- someting html -->
	</div>
</div>
```