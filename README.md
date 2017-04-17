# aggregation-query-and-display

A Polymer Element that builds and runs an elasticsearch aggregation query and shows the transformed results in a bar chart with optional selectable behavior.

### Example
```html
<aggregation-query-and-display
  aggregation-field="myAggregationField"
  query-field="myQueryField"
  query-value="myQueryValue"
  client="[[client]]"
  index-name="myIndexName"
  index-types='["myIndexType"]'
  filter-list="[[filterList]]"
  transform-config="{}"
  transform-function="[[myTransformFunction]]"
  show-checkboxes
  selected="{{selected}}">
</aggregation-query-and-display>
```

### Dependencies

Dependencies are installed using [Bower](http://bower.io/):

    npm install -g bower
    bower install

### Testing

Tests are run using [web-component-tester](https://github.com/Polymer/web-component-tester):

    npm install -g web-component-tester
    wct

### Demonstration & Documentation

Demonstration and documentation are viewed using [polyserve](https://github.com/PolymerLabs/polyserve):

    npm install -g polyserve
    polyserve

