# jvectormap-bulgarian-maps
Jvectormap bulgarian regions map


Demo:
-----------

http://heminei.github.io/jvectormap-bulgarian-maps/demo/

How to use:
-----------

```html
<script src="../libs/jquery-jvectormap-2.0.3/jquery-jvectormap-2.0.3.min.js" type="text/javascript"></script>
<script src="../src/jquery-jvectormap-bg-regions.js" type="text/javascript"></script>
```

```javascript
$(function () {
    var gdpData = {
        "BG342": 100,
        "BG321": 200,
    };
    $('#bg-map').vectorMap({
        map: 'bg_regions',
        series: {
            regions: [
                {
                    values: gdpData,
                    scale: ['#C8EEFF', '#0071A4'],
                    normalizeFunction: 'polynomial'
                }
            ]
        }
    });
});
```