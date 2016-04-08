This [choropleth](../4060606) uses a [threshold scale](https://github.com/mbostock/d3/wiki/Quantitative-Scales#wiki-threshold) for quantization, mapping arbitrary slices of a continuous domain to discrete values in the range. Unemployment rates ranging from 2 to 10% are quantized into different shades of purple.

```javascript
var color = d3.scale.threshold()
    .domain([0.02, 0.04, 0.06, 0.08, 0.10])
    .range(["#f2f0f7", "#dadaeb", "#bcbddc", "#9e9ac8", "#756bb1", "#54278f"]);
```
