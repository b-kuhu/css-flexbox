# Flex-wrap

### if we give width:300px then for 10 box elements, the total width comes out to be 3000px which is more than browser width. What flexbox does is that it takes that width is thta it takes that width and calculates the width that is currently available and distributes the currently available width equally to each box element.

### By default, the flex-wrap property is nowrap.

### If we use flex-wrap: wrap, then it says that okay , we have to stretch across our container to its full height but we also need to split it up between the 10 of us.So the browser calculates that it needs 4 rows and it will split it such that each row occupies 3 box elements.

### If we change it to flex-wrap: wrap-reverse, the direction from bottom to top but still the elements order in each row remains in the same direction as before i.e left to right.

### Now, if we change the flex direction: column, it will wrap all the box elements from top to bottom wrt its height ( here 100vh).After the height is occupied it will go towards right. This will also go from left to right for elements that are left.