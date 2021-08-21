# **Horiseon Refactoring**

I am updating the code base for better semantics, logical structure independent of styling and positioning, accessible alt attributes, sequential order, and a concise descriptive title. 

## **Progress**
**<u>08/20/2021</u>**
In index.html changed the title from "Website" to "Horiseon". Inside the body I made a couple of semantic changes by replacing the `<div class="header">` with just `<header>`. Then Replaced the `<div>` under `<h1>` tag to `<nav>`. There was a link issue inside the `<nav>` list's `Search Engine Optimization`, but this was resolved by adding an `id="search-engine-optimization"` in th body where this section is. The content section under `<div class="hero"></div>` I changed the `<div class="content">` to `<section class="content">` for better semantics and to avoid the div soup for this section of the webpage. 

The style.css file had a few changes, as well. The first change was changing the `.header {}` from this class selectors to the element selector `header {}` because we changed the the `<div class="header">` to just `<header>`. The only other thing that was changed is the `header nav {}, header nav ul {}, header nav ul li {}` where the `nav` replaced the `div` because we changed that tag in index.html for better semantics. Removing the unnecessary element selectors, `header h1`, and leaving the class selector, `.seo`. Moved items around and added comments to make it easier for me to go between index.html and style.css and not have to scramble through the style.css to find whats connected to index.html

**<u>08/21/2021</u>**
Index.html under the `<section class="content">`, I have added alt attributes to the `<img>`. Replaced the `<div class="benefits">` with `<section class="benefits">` for better semantics and to avoid having a div soup for this section. 

In style.css the class selectors, `search-engine-optimization`, `online-reputation-management`, `social-media-marketing`, and they're `img` and `h2` selectors have been compiled into three classes; `content div`, `content div img`, `content div h2`.