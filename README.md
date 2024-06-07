## Bootstrap Install

-   Include Bootstrap’s CSS and JS. Place the `<link>` tag in the `<head>` for our CSS, and the `<script>` tag for our JavaScript bundle (including Popper for positioning dropdowns, poppers, and tooltips) before the closing `</body>`.

```html
<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="utf-8" />
		<meta
			name="viewport"
			content="width=device-width, initial-scale=1" />
		<title>Bootstrap demo</title>
		<link
			href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css"
			rel="stylesheet"
			integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH"
			crossorigin="anonymous" />
	</head>
	<body>
		<h1>Hello, world!</h1>
		<script
			src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"
			integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz"
			crossorigin="anonymous"></script>
	</body>
</html>
```

### Viewport meta tag (very important)

-   Since Bootstrap is mobile first the viewport meta tag wil ensure that bootstrap works as intended on all device
    viewport width and heights.

```html
<meta name="viewport" content="width=device-width, initial-scale=1" />
```

### The Container:

The container is the fundamental building block of the Bootstrap 5 layout. It is used to center and align your content on the page, providing a responsive and fluid design. There are two types of containers in Bootstrap 5: the standard container and the fluid container.

-   Standard Container: Centers and aligns content with a fixed-width.
-   Fluid Container: Expands to fill the entire viewport, providing a fully responsive layout.

![alt text](grid-system.png)
[Container example](https://getbootstrap.com/docs/5.3/examples/grid/#containers)

### The Grid System:

Bootstrap 5 employs a powerful 12-column grid system to structure and organize content. This responsive grid system allows for easy layout creation by simply dividing the page into columns and rows using the following classes:

-   Container: Wraps the grid and provides a base structure.
-   Row: Defines a horizontal group of columns.
-   Column: Represents an individual column within the row.

The grid system also includes a series of responsive classes for different screen sizes:

![alt text](breakp.png)

-   Extra small (col): <576px
-   Small (col-sm): ≥576px
-   Medium (col-md): ≥768px
-   Large (col-lg): ≥992px
-   Extra large (col-xl): ≥1200px
-   Extra extra large (col-xxl): ≥1400px

### Flexbox and Alignment

Bootstrap 5 utilizes the power of Flexbox to provide more flexible and advanced layout options. It offers a variety of alignment classes to align content both vertically and horizontally within containers, rows, and columns.

-   Start: Aligns items to the start of the parent element.
-   Center: Centers items within the parent element.
-   End: Aligns items to the end of the parent element.
-   Baseline: Aligns items along their baselines.
-   Stretch: Stretches items to fill the available space.

### Spacing and Utility Classes:

Bootstrap 5 introduces a wide range of utility classes for managing margins, padding, and other layout properties. These classes follow a simple syntax, making it easy to apply consistent spacing throughout your design:

-   “m” for margin, “p” for padding
-   “t” for top, “b” for bottom, “l” for left, “r” for right, “x” for horizontal, “y” for vertical
-   0-5 for spacing values

For example, to apply a margin of 3 units to the top and bottom of an element, you would use the class “my-3”.

### Responsive Breakpoints

In order to provide optimal user experiences across various devices, Bootstrap 5 features predefined breakpoints that allow you to define different styles for different screen sizes. The breakpoints can be used in conjunction with the grid system and other Bootstrap layout components to create responsive designs.
