# Short Response Questions

Answer the following questions in 2-4 sentences each. Be specific and use vocabulary from the lessons.

## Question 1: Flexbox Basics

What is the difference between a **flex container** and a **flex item**? How do you make an element a flex container?

A flex container is an element that has its display property set to flex or inline-flex, which allows its direct children to be arranged using the Flexbox layout model. A flex item is any direct child of a flex container that can be positioned and sized along the container’s main and cross axes. To make an element a flex container, you apply display: flex; or display: inline-flex in its CSS. This allows you to use properties like justify-content, align-items, and flex-direction to control the layout of its flex items.

## Question 2: Main Axis vs Cross Axis

In Flexbox, what is the **main axis** and what is the **cross axis**? How do `justify-content` and `align-items` work with these axes?

In Flexbox, the main axis is the default direction that the flex items are laid out, which is determined by the flex-direction property. The flex-direction is set to row by default and runs horizontally, column runs vertically. The cross axis is perpendicular to the main axis which is vertical if the main axis is horizontal, and horizontal if the main axis is vertical. The justify-content property aligns flex items along the main axis, controlling spacing and distribution, while align-items aligns items along the cross axis, controlling how they line up perpendicular to the main direction.

## Question 3: Flexbox vs Grid

When would you use **Flexbox** vs **CSS Grid**? Give an example of a layout that would be better suited for each.

You would use Flexbox when you need to arrange items in a single row or column with flexible spacing or alignment. One example is a navigation bar with evenly spaced links is best done with Flexbox because it easily handles horizontal alignment and spacing.
You would use CSS Grid when you need a two-dimensional layout that controls both rows and columns simultaneously. For example, a product gallery with multiple rows and columns of cards is better suited for Grid because it allows precise placement of items in both directions.

## Question 4: The `fr` Unit

What does the `fr` unit do in CSS Grid? Explain what `grid-template-columns: 1fr 2fr 1fr` would create.

In CSS Grid, the fr unit represents a fraction of the available space in the grid container. It lets you divide the container into even sections rather than fixed sizes.
For example, grid-template-columns: 1fr 2fr 1fr; creates three columns where the first and third columns each take 1 fraction of the available space, and the middle column takes 2 fractions, making it twice as wide as the outer columns.

## Question 5: Media Queries

What is a **media query** and why are they important for **responsive web design**? Write an example of a media query that applies styles for screens 768px and wider.

A media query is a CSS rule that applies styles only when certain conditions about the user’s device or viewport are met, such as screen width or height. They are important for responsive web design because they allow a website to adjust its layout and styling for different devices, like phones, tablets, and desktops. This is so that content looks good and is easy to use on any screen size.

```css
@media (min-width: 768px) {
  .products-container {
    grid-template-columns: repeat(2, 1fr);
    gap: 20px;
  }
}
```

## Question 6: Mobile-First Design

What does **mobile-first design** mean? What are the benefits of taking a mobile-first approach versus a desktop-first approach?

Mobile-first design means designing a website starting with the smallest screens like smartphones and then progressively adding styles for larger screens using media queries. This approach ensures that the core content and functionality work well on mobile devices before adding enhancements for tablets or desktops.
The benefits of mobile-first design include better performance, since mobile users get only the essential styles and content first, and easier scalability, because layouts naturally adapt to larger screens.
