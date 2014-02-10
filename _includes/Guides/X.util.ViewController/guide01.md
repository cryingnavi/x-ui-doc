## X.util.ViewController (#viewcontroller)
X.View 의 프로퍼티로 추가할 수 있는 util입니다. 해당 view의 화면 전환 및 히스토리를 관리하게 됩니다. 예를 들어 view의 내용을 a.html 의 내용으로 채우고 싶고 이를 다시 a.html -> b.html 로 화면이 전환된다면 viewController를 선언하여 추가함을 써 이를 수행합니다.

또한 View 에 ViewController 가 추가되면 view 자신이 내포하고 있는 html 중, 링크 태그를 클릭하였을 경우 href로 명시된 url로 자동으로 페이지가 전환됩니다.

전환시에는 애니메이션이 동작합니다.

[X.util.ViewController](./assets/x-ui-1.0.3/doc/X.util.ViewController.html)

ViewController 는 하위로 다음 두 클래스를 가지고 있습니다.
+ X.util.LocalViewController : 이미 생성된 view들 간의 전환
+ X.util.RemoteViewController : 별도의 html 파일로의 전환


#### X.util.LocalViewController
이미 생성된 view 를 LocalViewController 에 등록하여 이들 간의 화면 전환을 담당합니다.

```javascript
var view = new X.View({
	el: "#detail-container",
	autoRender: true,
	viewController: new X.util.LocalViewController({
		initPage: "a.html"
	})
});
```

```html
<div data-ui="view" data-scroll="false" id="detail-container">
	        
</div>

<script>
X.util.cm.get("detail-container").setViewController(new X.util.LocalViewController({
	initPage: "a.html"
}));
</script>
```


#### X.util.RemoteViewController
별도의 html 파일로 나눠져 있는 페이지로 이동합니다.

```javascript
var view = new X.View({
	el: "#detail-container",
	autoRender: true,
	viewController: new X.util.RemoteViewController({
		initPage: "a.html"
	})
});
```

```html
<div data-ui="view" data-scroll="false" id="detail-container">
	        
</div>

<script>
X.util.cm.get("detail-container").setViewController(new X.util.RemoteViewController({
	initPage: "a.html"
}));
</script>
```
