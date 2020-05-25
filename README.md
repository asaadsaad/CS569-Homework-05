# CS569 Homework 06
## Exercise
1. Create a custom directive called `isVisible` that accepts a boolean which is going to show or hide the element.
```html
<component [isVisible]="false"></component> <!-- should be hidden -->
```
2. Create a custom directive called `makeBigger` that increases the size of the text by `2px` every time users double-click on the host element. 
```html
<component makeBigger></component> 
<!-- when double-click the component, it will increase its size -->
```
3. Create a custom pipe `multi` that works on strings and receives one number to repeat the string number of times, example: `string | multi:3` will result to: `string string string`
```javascript
@Component({template: `{{name | multi:5}}`}) // it will render the property `name` 5 times
```
