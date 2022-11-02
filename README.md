# CS569 Homework
## Exercise
1. Create a custom directive called `colorize` that is going to set the font color value of the host component text to a random color value every 1 second. Colors array is defined in the directive state: `['red', 'blue', 'green', 'yellow', 'maroon'....etc]`. Make sure your code does not lead to a memory leak (implement ngOnDestroy to clear your interval).
```html
<p colorize>This text will change color every second</p>
```
2. Create a custom directive called `makeBigger` that increases the size of the host element text by `n` pixels passed as an input property to the directive every time users double-click on the host element. 
```javascript
@Component({
  selector: 'app-root',
  template: `
    <p [makeBigger]="size1"></p> 
    <!-- when double-click the paragraph, it will increase its size by 2px -->

    <p [makeBigger]="size2"></p> 
    <!-- when double-click the paragraph, it will increase its size by 6px -->
`})
class AppComponent{
  size1 : number = 2;
  size2 : number = 6;
}

```
3. Create a custom pipe `swapLetter` that works on strings and receives two letters, one to look for and replace it with the other letter. Example:
```javascript
@Component({template: `{{'Asaad' | swapLetter:'a':'@'}}`}) // it will render `@s@@d`
```
