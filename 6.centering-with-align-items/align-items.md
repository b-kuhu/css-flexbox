
## align-items is more concerned with the cross-axis i.e it works top to bottom.It will work only if their exists some height vertically. 

### Lets say we use 

```css
    display: flex;
    align-items: center;
```
#### Their will be no change since vertically the height occupied will be only that of the elements. So no room for cenetering.

### If we give it a height 100vh,then it works as expected aligned to the center vertically
```css
    display: flex;
    height: 100vh
    align-items: center;
```
## Types of properties in align-items:
### a)stretch(default) : stretches to the full length of the container
### b)center - aligns to the center of the cross axis
### c)flex-start - aligns to the start of the cross-axis
### d)flex-end - aligns to the end of cross-axis.
### e)baseline: It looks at the text in your items and make your the bottom of every text,bottom,number is aligned at the same line.

#### If we change the font-sizes of some boxes as below:
```css
.box1{
    font-size: 20px;
}
.box3{
    font-size: 150px;
}
.box9{
    font-size:10px
}
```
#### The text of each box remains aligned remains on the same line still.

#### If we change the flex-direction to column, now the direction will be left to right ie main axis and items will be stacked above each other.

```css
.container{
    display: flex;
    height: 100vh;
    align-items: center;
    flex-direction: column;
}

```