# Archie 🐶
Mobile-first flex grid that falls back to a block layout where flex isn't supported. Specialises in equal width and odd columns e.g. fifths but also offers varied width columns.

# Features
1. Falls back to block layout where flex isn't supported.
2. Auto-columns - 1 column per element, akin to Foundation's XY grid.
3. Equal width columns , e.g. halves, thirds, fourths, fifths. Easily extendable.
4. 12 column grid with simple syntax, e.g. grid__6 is half the space, similar to Bootstrap's grid.
5. Mobile-first, just like to Tailwind's utility classes for creating layouts.
6. Responsive - uses breakpoints 640px (sm), 768px (md), 1025px (lg), 1280px (xl), and can be customised and extended.
7. Keeps markup clean - if you want to avoid littering your HTML width class names, Archie uses a universal for selection of equal width column grids. This means you don't need to add class names to child elements. The lower specificity is also easier to override.
8. Keeps markup semnatic - you can use the classes with lists, articles, sections, and more.
9. Easy to add custom, responsive gutters. Add grid modifier classes for horizontal and vertical padding using the universal column selector to target all columns, then add negative margin equal to these amounts on the grid modifier class. This ensures columns remain flush with the grid element.
10. No reliance on Sass / Less files. I've added source CSS and minified CSS files.

# Download
You may add the archie.min.css file straight to your project or you may wish to download the archie.css file to make modifications easier. You should minify your CSS and consider using a plugin such as Purge CSS if you use it in production.

# Questions?
From linting, I noticed that the universal selector is discouaged as it is known to be slow. However, I have found a number of sources that seem to convey that its impact is negligible to users.

https://stackoverflow.com/questions/2951997/what-is-the-performance-impact-of-the-universal-selector
https://www.telerik.com/blogs/css-tip-star-selector-not-that-bad
https://alistapart.com/article/axiomatic-css-and-lobotomized-owls/
http://www.stevesouders.com/blog/2009/03/10/performance-impact-of-css-selectors/
https://benfrain.com/css-performance-revisited-selectors-bloat-expensive-styles/

I have personally found that the more specific CSS is, the harder it is to maintain and extend. That's why I opted for the use of the universal selector. However, you are welcome to find and replace instances of this selector and change them to a classname of your choice.

# Why's it called Archie?
I have a dog now! His name is Archie 🐶

