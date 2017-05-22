#  ng-datespan-validator
![alt text](http://findicons.com/files/icons/2773/pictonic_free/128/angularjs.png) 
Component to validate time span between start dates and end dates.


## Bower

```
bower install dvalidate --save
```

## Adding Dependency.

```javascript
angular.module('app', ['dvalid']);
````

## DOM 

```html
<form name="myForm"> 
      <div dvalidate 
        init="your-startdate-ngmodel" 
        end="your-enddate-ngmodel" 
        ng-model="validated-ngmodel"> 
        </div>
</form>
```


### Example


include the package.
```javascript
    <script src="bower_components/dvalidate/dvalid.min.js"></script>
```


In your form,

```html

<form name="myForm">

    <input type="date" ng-model="init">
    <input type="date" ng-model="end">

    <div dvalidate init="init" end="end" ng-model="validation"></div>

    <pre>
        {{myForm.$error | json}}
    </pre>
</form>

```



### Note: 
timestamps are not validated.
