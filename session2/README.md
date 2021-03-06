
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

The scale function not only can transform **number** into **number**, it can also take an input of **category** or **date**, and make an output of **color** or **coordinates**. 

We are going to follow the tutorial here to learn about different types of scales: 
http://d3indepth.com/scales/ 

And then, we will use three different scales to recreate this graphic: http://graphics.wsj.com/in-polling-who-got-it-right/

## How to define a scale when the data is dynamic?
### d3.min
```d3.min(data, function(d){ return d["repMinusDemDiff"]})```

### d3.max
```d3.max(data, function(d){ return d["repMinusDemDiff"]})```

### d3.extent
```colorScale.domain([d3.min(data, function(d){ return d["repMinusDemDiff"]}), 0, d3.max(data, function(d){ return d["repMinusDemDiff"]})])```

## Readings: 
https://www.dashingd3js.com/d3js-scales 
