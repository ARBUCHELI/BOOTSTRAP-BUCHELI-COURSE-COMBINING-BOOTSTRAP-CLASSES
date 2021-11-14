# BOOTSTRAP-BUCHELI-COURSE-COMBINING-BOOTSTRAP-CLASSES

In the previous exercise, we went over how to follow Bootstrap naming conventions to add breakpoint requirements for a column. We can go one step further and add multiple classes to our columns for additional control over the rendering of our content.

Let’s walk through the syntax and thought process using an example:

First, we’d want to think about how our column looks like on extra small screens. Since we don’t have much space, we would want to have our column take up the entirety of the row and assign a class of "col-12". We don’t include an xs breakpoint, it’s implicitly applied for us! Our column looks like:

```
<div class="col-12">
</div>
```
Then we decide that for medium-sized screens we don’t want the column to take up so much space, so we could set the width to 8. We use the Bootstrap naming convention and add an additional class to the column like so:

```
<div class="col-12 col-md-8">
</div>
```
For large screen sizes, we want the column to take up even less relative space and we set the width to 6. We have to add another class to the column:

```
<div class="col-12 col-md-8 col-xl-6">
</div>
```
From the example, we have a column that renders a different width based on a user’s screen size. On extra small and small sized screens, the column has a width of 12 individual columns. For medium and large sized screens, the column has a width of 8 individual columns. Lastly, for extra large screens, the column has a width of 6 individual columns. We could’ve even used up all of Bootstrap’s provided breakpoints! Read Bootstrap’s grid mix and match documentation for more information.

## Take a look at the live example here:
https://bucheli-web-development-bootstrap-course-combining-classes.netlify.app/
