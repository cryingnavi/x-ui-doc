## 레이아웃 만들기 (#layout)
X.View 들 간의 관계를 통해 다양한 레이아웃을 만들어 낼 수 있다. 레이아웃을 만드는데 필요한 속성은 `data-layout` 와 `data-flexible` 두 속성이다.

+ Header / Body

<img src="./images/layout01.png" width="200" height="170"/>

```html
<!-- header -->
<div data-ui="view" data-flexible="false" style="height: 60px;">
	<!-- someting html -->
</div>

<!-- body -->
<div data-ui="view">
	<!-- someting html -->
</div>	
```

+ Header / Body / Footer

<img src="./images/layout02.png" width="200" height="170"/>

```html
<!-- header -->
<div data-ui="view" data-flexible="false" style="height: 60px;">
	<!-- someting html -->
</div>

<!-- body -->
<div data-ui="view">
	<!-- someting html -->
</div>

<!-- footer -->
<div data-ui="view" data-flexible="false" style="height: 60px;">
	<!-- someting html -->
</div>
```


3. Left / Body

<img src="./images/layout03.png" width="200" height="170"/>

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


4. Left / Body / Right

<img src="./images/layout04.png" width="200" height="170"/>

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

	<!-- right -->
	<div data-ui="view" data-flexible="false" style="width: 100px;">
		<!-- someting html -->
	</div>
</div>
```


5. Header / Body / Footer / Left / Right

<img src="./images/layout05.png" width="200" height="170"/>

```html
<!-- header -->
<div data-ui="view" data-flexible="false" style="height: 100px;">
	<!-- someting html -->
</div>

<div data-ui="view" data-layout="x">
	<!-- left -->
	<div data-ui="view" data-flexible="false" style="width: 100px;">
		<!-- someting html -->
	</div>

	<!-- body -->
	<div data-ui="view">
		<!-- someting html -->
	</div>

	<!-- right -->
	<div data-ui="view" data-flexible="false" style="width: 100px;">
		<!-- someting html -->
	</div>
</div>

<!-- footer -->
<div data-ui="view" data-flexible="false" style="height: 100px;">
	<!-- someting html -->
</div>
```