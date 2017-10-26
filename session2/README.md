
```js
//adding y axis
svg.append("g")
   .attr("transform", "translate(" + margin.left + "," + margin.top + ")")
   .call(d3.axisLeft(yScale).tickFormat(d3.format("$,")))
   
//adding x axis
svg.append("g")
   .attr("transform", "translate(" + margin.left + "," + (height + margin.top) + ")")
   .call(d3.axisBottom(xScale));
```

## Scale functions: 
“Scales are functions that map from an **input domain** to an **output range**.” 

In the case below, we are transforming input data between (and including) 0 and 10,000, into output data between (and including) 0 and 100.

Visually, we want to do the following: 

![alt text](https://s3.amazonaws.com/dashingd3js/images/d3.js_scales_scale_domain_down_to_range_300x300.png "")

### d3.scaleLinear()

### d3.min

### d3.max


## Readings: 
https://www.dashingd3js.com/d3js-scales 
