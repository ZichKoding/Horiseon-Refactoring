# **Horiseon Refactoring**

I am updating the code base for better semantics, logical structure independent of styling and positioning, accessible alt attributes, sequential order, and a concise descriptive title. 

## **Progress**
**<u>08/20/2021**
In index.html changed the title from "Website" to "Horiseon". Inside the body I made a couple of semantic changes by replacing the `<div class="header">` with just `<header>`. Then Replaced the `<div>` under `<h1>` tag to `<nav>`. There was a link issue inside the `<nav>` list's `Search Engine Optimization`, but this was resolved by adding an `id="search-engine-optimization"` in th body where this section is.

The style.css file had a few changes, as well. The first change was changing the `.header {}` from this class selectors to the element selector `header {}` because we changed the the `<div class="header">` to just `<header>`. The only other thing that was changed is the `header nav {}, header nav ul {}, header nav ul li {}` where the `nav` replaced the `div` because we changed that tag in index.html for better semantics. 