#### Examples of Binding
__2-way binding__
```
<input type="text" ng-model="name">
```
_2-way binding (ng-model) means:_
* _listener for change on input automatically set up by Angular updates prop value on $scope_
* _direct update to prop value is automatically updated in UI_

__1-way binding__
```
<div>Echo: {{lastName}} </div>
```
_1-way binding ({{prop}}) means:_
* _direct update to prop value is automatically updated in UI_

__1-time binding__
```
<div>Echo: {{::fullName}} </div>
```
_1-time binding ({{::prop}}) means:_
* _initialized value of prop is automatically updated in UI_
* _watcher for prop is removed, so UI never again gets updated_