##Alert是个人娱乐的一个弹出框插件

Alert包含了常用的alert,comfirm,prompt这三种弹出层提示语。本插件兼容commentJs/AMD/CMD规范

##Alert的大小为4.6k内部有一个rem的算式。
插件中的css单位都为rem 其默认大小及说明在下方将会说明。

##Alert的使用如下:

* rem的单位计算
```javascript
	let designSize = 750;   // 此处为设计图的宽度 开发人员请参照实际情况赋值
	let yourRatio = 100;    // yourRatio为你自己的缩放比例 此处设为100时 若设计图为70px 则你的css大小为0.7rem;
	rem.init(750,100);      // 在控制台可以看到当前的fontSize;
```

* 普通的alert弹出层
```javascript
	Alert.alert('your message',function () {     // 此处为两个参数 一、你希望展现的文字; 二、确定之后的回调;
		// if the choice is determineddo do something;
		});
```

* confirm弹出层
```javascript
	Alert.confirm('your message',function () {       // 此处为三个参数 一、你希望展现的文字; 二、确定之后的回调; 三、取消之后的回调;  
		// if the choice is determined do something;
		},function() {
		// if the choice is cancelled do something;
		});
```

* prompt弹出层  注: `data`为用户填写完成后的输入值
```javascript
	Alert.prompt('your message',function (data) {     // 此处为三个参数 一、你希望展现的文字 二、确定之后的回调  三、取消之后的回调;
		// if the choice is determineddo do something;
		},function () {
		// if the choice is cancelled do something;
		});
```


##关于作者
一个初学者