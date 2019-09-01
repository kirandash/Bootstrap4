# Bootstrap 4
## 1. Intro
### 1.1 Installation
Current version: 4.3.1
1. CSS and JS
2. Boostrap CDN
3. Source files
4. Package managers

https://getbootstrap.com/docs/4.3/getting-started/download/
Download compiled css and js folder
css folder - .map files helps us point to sass files in development mode
.reboot files - resets browser specific styles

js folder - bootstrap.bundle file contains = bootstrap code + popper js

### 1.2 Template Creation
Start with starter template
https://getbootstrap.com/docs/4.3/getting-started/introduction/
Development mode: Use local css, js files for libraries.
Prod mode: Use cdn

## 2 Basic styles
### 2.1 Basic Styles Intro
Bootstrap uses reboot for normalization. It uses rem unit ie. 1rem = 16px; for normalization while other normalization rules uses px for normalization

### 2.2 Basic Typography
Default bootstrap 4 behavior
1. Reboot.css
2. Rems vs ems
3. Avoid margin-tops
4. inherit when possible
5. border-box sizing
6. Native font stacks
7. Special styles

classes:
1. h1,h2,h3...
2. display-1, display-2, display-3, display-4 (bigger than h1, h2, h3 ....)
3. p class="lead" - lead paragraph
4. tags: <small>, <del>, <em>

### 2.3 Typographic utilities
1. text-justify
2. text-(size)-POS e.g. text-lg-center, 
3. align-SID e.g. align-baseline, align-top, align-bottom, etc
4. text-TYP e.g. text-uppercase, text-lowercase
5. font-STYL e.g. font-italic, font-weight-normal, font-weight-light etc.
6. text-decoration-none
7. text-reset: removes texts color and inherits from parent container
8. text-flow: text-wrap, text-nowrap, text-break, text-truncate (creates ellipsis for longer texts)
9. bg-warning

### 2.4 Blockquotes and lists
1. list-unstyled: no bullets
2. list-inline: on ul and list-inline-item on li
3. blockquote, blockquote-footer, blockquote-reverse

### 2.5 Colors
1. text-color: text-success, text-danger, text-warning etc.
2. bg-COLOR: bg-primary, bg-success, bg-danger etc.

### 2.6 Images
1. img-fluid: responsive images
2. img-thumbnail: rounded 1px border
3. rounded-SIDE or -SHAPE or -SIZE e.g. rounded-top, rounded-circle, rounded-pill, rounded-sm, rounded-lg, rounded-0
4. float-left, float-right, text-center, mx-auto: to center block images
5. figure, figure-img, figure-caption

### 2.7 CSS variables
New feature. Browser compatibility
var() and :root
Ex: 
:root{ 
    --yellow: #C4226F; 
    --danger: #FFBA00;
}; // redefining variable
color: var(--yellow); //using variable
color: var(--danger);