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
