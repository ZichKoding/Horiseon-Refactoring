# **Horiseon Refactoring**

I have been assigned to update the codebase for better semantics, logical structure independent of styling and positioning, accessible alt attributes, and sequential order. This is to be more modern for people visiting the site that rely on text-to-speech technology to read the site, or anyone else that uses assistive technology. 

[Horiseon's website](https://zichkoding.github.io/Horiseon-Refactoring)

![Top of Horiseon Website](./assets/images/Horiseon.png)

## **Progress**
**<u>08/20/2021</u>**

In index.html changed the title from "Website" to "Horiseon". Inside the body I made a couple of semantic changes by replacing the `<div class="header">` with just `<header>`. Then Replaced the `<div>` under `<h1>` tag to `<nav>`. There was a link issue inside the `<nav>` list's `Search Engine Optimization`, but this was resolved by adding an `id="search-engine-optimization"` in th body where this section is. The content section under `<div class="hero"></div>` I changed the `<div class="content">` to `<section class="content">` for better semantics and to avoid the div soup for this section of the webpage. 

The style.css file had a few changes, as well. The first change was changing the `.header {}` from this class selectors to the element selector `header {}` because we changed the the `<div class="header">` to just `<header>`. The only other thing that was changed is the `header nav {}, header nav ul {}, header nav ul li {}` where the `nav` replaced the `div` because we changed that tag in index.html for better semantics. Removing the unnecessary element selectors, `header h1`, and leaving the class selector, `.seo`. Moved items around and added comments to make it easier for me to go between index.html and style.css and not have to scramble through the style.css to find whats connected to index.html

**<u>08/21/2021</u>**

Index.html under the `<section class="content">`, I have added alt attributes to the `<img>`. Replaced the `<div class="benefits">` with `<section class="benefits">` for better semantics and to avoid having a div soup for this section. Benefits section I have added alt attributes to the images, but left them blank due to not knowing how to describe these images or if they are worth describing. In the benefits section I have took away the classes except for `benefits`. The `<div class="footer">` was replaced by the semantic tag, `<footer>`.

In style.css the class selectors, `search-engine-optimization`, `online-reputation-management`, `social-media-marketing`, and they're `img` and `h2` selectors have been compiled into three classes; `content div`, `content div img`, `content div h2`. There was a similar section under benefits and I compiled the 9 classes into 3 classes called, `.benefits div`, `.benefits div h3`, and `benefits div img`.