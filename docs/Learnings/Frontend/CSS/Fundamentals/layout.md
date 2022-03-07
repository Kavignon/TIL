# CSS Layout

A good resource that I've found is [this](https://www.youtube.com/watch?v=yMEjLBKyvEg)

## CSS Size & Units

    - Intrinsic vs extrinsic sizing: In the case of intrinsic sizing, the UI element must consider the content it holds and decide how big it needs to be to make sure it can hold it. In short, intrinsic sizing simply wants something big enough to fit the given content. In the case of extrinsic size, we're specifying the dimensions of the UI element and we'll be focused on fitting it in the provided scope.

    * It's use for everything that has to scale according to the font size.

    - Pixels (px): It is an absolute unit of measurement. Because it is an absolute measurement, it may be used any time you want to define something to be a particular size, rather than being proportional to something else like the size of the browser window or the font size. Because many browsers support custom font sizes, which would override the CSS of the website, designing with pixels could lead to something breaking.

    - Em: Em is not an absolute unit - it is a unit that is relative to the currently chosen font size. Unless you have overridden font style by setting your font size with an absolute unit (ex: px), this will be affected byu the choice of the fonts in the user's browser or OS if they have made one, so it does not make sense to use em as a general unit of length except where you specifically want it to scale as the font size scales.

    - Auto: It is essentially a kind of intrinsic sizing. It defines the dimensions of the of the layout based on the content it holds.

## CSS Grid

    - Grid cell: The smallest area that you can find in the grid.
    - Gap: Can be used to provide space gaps for all grid cells inside the grid.
    - Implicit grid: If you define the container to be a grid and you don't specify the grid-template for rows and columns, the display comes with an implicit grid by default. The grid will create implicit tracks for you. Based on the recommendation of the video, it seems that most of the time, we'd want to control the column's template and let the implicit grid take care of the rows. The rows will be be as big as they need to be to support the content. When defining the tracks in the grid, they are set by default to auto, so they should be big enough to fit the content that you'll provide.
