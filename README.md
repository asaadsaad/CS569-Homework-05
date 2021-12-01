# CS569 Homework 05
## Exercise
1. Create a custom directive called `colorize` that is going to set the font color value of the host component text to a random color value every 1 second. Colors are predefined in the state as an array: `['red', 'blue', 'green', 'yellow', 'maroon'....etc]`. Make sure your code does not lead to a memory leak.
```html
<component colorize></component> <!-- the text will change color every second -->
```
2. Create a custom directive called `makeBigger` that increases the size of the text by `n` pixels passed as an input every time users double-click on the host element. 
```html
<component [makeBigger]="2"></component> 
<!-- when double-click the component, it will increase its size by 2px -->

<component [makeBigger]="6"></component> 
<!-- when double-click the component, it will increase its size by 6px -->

```
3. Create a custom pipe `swapLetter` that works on strings and receives two letters, one to look for and replace it with the other letter.
```javascript
@Component({template: `{{'Asaad' | swapLetter:'a':'@'}}`}) // it will render `@s@@d`
```
