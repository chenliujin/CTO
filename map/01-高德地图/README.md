


# [点标注](http://lbs.amap.com/api/javascript-api/guide/draw-on-map/marker-point)

## 点聚合
context 有三个属性：count/marker/markers，count是markers的总个数，marker为聚合后的点，markers（数组）是聚合前的所有点；

```
  var count  = markers.length;
    var _renderCluserMarker = function (context) {
      console.log(context.markers[0].getContent());
      
        var factor = Math.pow(context.count/count,1/18)
        var div = document.createElement('div');
        var Hue = 180 - factor* 180;
        var bgColor = 'hsla('+Hue+',100%,50%,0.7)';
        var fontColor = 'hsla('+Hue+',100%,20%,1)';
        var borderColor = 'hsla('+Hue+',100%,40%,1)';
        var shadowColor = 'hsla('+Hue+',100%,50%,1)';
        div.style.backgroundColor = bgColor
        var size = Math.round(30 + Math.pow(context.count/count,1/5) * 20);
        div.style.width = div.style.height = size+'px';
        div.style.border = 'solid 1px '+ borderColor;
        div.style.borderRadius = size/2 + 'px';
        div.style.boxShadow = '0 0 1px '+ shadowColor;
        div.innerHTML = context.count;
        div.style.lineHeight = size+'px';
        div.style.color = fontColor;
        div.style.fontSize = '14px';
        div.style.textAlign = 'center';
        context.marker.setOffset(new AMap.Pixel(-size/2,-size/2));
        context.marker.setContent(div)
        
        
     }
    addCluster(2);
```
