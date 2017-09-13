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

### Styling

`<aggregation-query-and-display>` provides the following custom properties and mixins for styling:

Custom property                                                | Description                                                         | Default
---------------------------------------------------------------|---------------------------------------------------------------------|--------
`--aggregation-query-and-display-bar-color`                    | The color of the single or left bars.                               | --paper-grey-400
`--aggregation-query-and-display-bar-count-color`              | The color of the single or left count labels.                       | --paper-grey-900
`--aggregation-query-and-display-bar-height`                   | The height of the single or left bars.                              | 20px
`--aggregation-query-and-display-bar-title-color`              | The color of the single or left title labels.                       | --paper-grey-900
`--aggregation-query-and-display-bar-title-hover-color`        | The color of the single or left title labels on hover (if a link).  | --paper-grey-700
`--aggregation-query-and-display-second-bar-color`             | The color of the right (second) bars.                               | --paper-grey-400
`--aggregation-query-and-display-second-bar-count-color`       | The color of the right (second) count labels.                       | --paper-grey-900
`--aggregation-query-and-display-second-bar-height`            | The height of the right (second) bars.                              | 20px
`--aggregation-query-and-display-second-bar-title-color`       | The color of the right (second) title labels.                       | --paper-grey-900
`--aggregation-query-and-display-second-bar-title-hover-color` | The color of the right (second) title labels on hover (if a link).  | --paper-grey-700

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

