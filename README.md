# simpleAngularUI
This repository contains a set of native AngularJS directives based on Bootstrap's markup and CSS.

# Installation
Angular Bootstrap TimePicker directive

To install TimePicker, run the following command in the Package Manager Console
```sh
PM> Install-Package simpleAngularUI
```


# TimePicker

All settings can be provided as attributes in the `sui-time-picker`



```html
<div class="container" ng-app="simpleAngularUI" ng-controller="myCtrl">
        <div class="row">
            <div class="col-md-6">
                <sui-time-picker time="timeConfig.time" string-time="timeConfig.stringTime" has-second="true"></sui-time-picker>
                {{timeConfig.time}}
            </div>
        </div>
    </div>
```
```js
app.controller("myCtrl", function ($scope) {
    $scope.timeConfig = {
        time: { h: 10, m: 0, s: 0 },
        stringTime: false
        };
    });
```

- [`time`]: In two ways:
     - Object Time: [`string-time`] property is `false`
     - String Time: [`string-time`] property is `true`

