## flex: 1 consists of three properties combined : 

## a) flex-grow : when we have extra space on our page,then how do we divide it among everybody on the same line.
## b) flex-shrink : shrinks when the space is less and divide it among everybody on the same line
## c) flex-basis : For eg : if we set our flex-basis for both the boxes to be 400px then it means that in an ideal world both the container will have 400px each width ie 800px total width . If the page width goes less than 800px, then flex-shrink will come into picture 

```css
.box1{
    flex-basis:400px;
    flex-shrink:10;
}
.box2{
    flex-basis:400px;
    flex-shrink:1;
}
```
#### the default for flex-shrink is 1. flex-shrink : 10 means box1 will shrink 10 times more than box2 when the width is reduced.

### We can also write all the three properties combined as flex : grow shrink basis
```css
.box1{
   flex: 1 10 400px;
}
.box2{
    flex: 1 1 400px;
}
```