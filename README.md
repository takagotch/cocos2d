### cocos2d
---
https://github.com/cocos2d

http://cocos2d.org/

```js
// tests/js-tests/src/ClippingNodeTest/ClippingNodeTest.js
var TAG_TITLELABEL = 1;
var TAG_SUBTITLELABEL = 2;
var TAG_SITECLINODE = 100;
var TAG_CLIPPERNODE = 101;
var TAG_CONTENTNODE = 102;

var clippingNodeTEstSceneIdx = -1;

var BaseClippingNodeTest = BaseTestLayer.extend({
  _title:"",
  _subtitle:"",
  
  ctor:function() {
    this._super(cc.color(0,0,0,255), cc.color(98,99,117,255));
    this.setup();
  },
  
  onRestartCallback:function (sender) {
    var s = new ClippingNodeTEstScene();
    s.addChild(restartClippinNodeTest());
    director.runScene(s);
  },
  onNextCallback:function (sender) {
    var s = new ClippingNodeTestScene();
    s.addChild(nextClippingNodeTest());
    director.runScene(s);
  },
  onBackCallback:function (sender) {
    var s = new ClippingNodeTestScene();
    s.addChild(previousClippingNodeTest());
    director.runScene(s);
  },
  
  numberOfPendingTests:function() {
    return ( (arrayClippingNodeTest.length-1) - clippingNodeTestSceneIdx );
  },
  
  getTestNumber:function() {
    return clippingNodeTestSceneIdx;
  }
});



```

```
```

```
```


