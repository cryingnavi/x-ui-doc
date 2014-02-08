## Getting Started
이 문서는 x-ui 의 핵심 개념에 대해 설명합니다.


#### MarkUp
```html
<!doctype html>
<head>
	<meta charset="utf-8">
	<title>Test Application</title>
	<link rel="stylesheet" type="text/css" href="x-ui.css" />
	<link rel="stylesheet" type="text/css" href="x-ui-theme.css" />

	<script type="text/javascript" src="jquery-1.10.2.min.js"></script>
	<script type="text/javascript" src="x-ui-min.js"></script>
	<script type="text/javascript" src="x-scroll.js"></script>
	<script type="text/javascript">
		X.App({
			ready: function(appView){
				appView.setContent();
			}
		});
	</script>
</head>
<body>
	
</body>
</html>
```


#### Include
```html
<link rel="stylesheet" type="text/css" href="x-ui.css" />
<link rel="stylesheet" type="text/css" href="x-ui-theme.css" />

<script type="text/javascript" src="jquery-1.10.2.min.js"></script>
<script type="text/javascript" src="x-ui-min.js"></script>
<script type="text/javascript" src="x-scroll.js"></script>
```
+ x-ui.css, x-ui-theme.css 등의 관련 css를 include 한다.
+ jquery-1.10.2.min.js, x-ui-min.js, x-scroll.js 를 include 한다.


#### Application 생성
```javascript
X.App({
	ready: function(appView){
		//application init
		appView.setContent();
	}
});
```
X.App 는 어플리케이션에 대한 생성 정보를 기술하는 method 이다. 상세 프로퍼티들은 다음 url 에서 확인할 수 있다.

[X.App](/assets/x-ui-1.1.1/doc/X.html#toc8)

`appView` 는 X.App 에 의해 최상위 body를 대상으로 생성한 `X.View`의 인스턴스의 참조를 담고 있다. 해당 view 객체의 setContent() method 를 호출하여 body 의 자식 태그들 중 data-ui 를 기술한 div를 읽어 해당 컴포넌트로 자동 생성한다.
