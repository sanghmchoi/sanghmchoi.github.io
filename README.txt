112121

A Jekyll Image Gallery
https://github.com/opieters/jekyll-image-gallery-example/tree/gh-pages

Moving
https://github.com/huangyz0918/moving

A Jekyll Image Gallery on top of Jekyll theme 'moving'.

'moving' by default comes with a css to enclose photos inside a round padded border, and it deems to be ugly when scaled up via lightGallery.
-> Overridden 'img' part of the '_sass/moving/_base.scss' with that of 'Jekyll Image Gallery''s. 
-> Overriding only the partials(moving/base) without its parent(moving) importing them in its code blocks, even when its parent is not modifed at all, doesn't take any effect.

'_includes/head.html' contains the code blocks to load up necessary plugins (lightGallery, isotope, masonry)

'_includes/gallery-layout.html'
-> Can no longer load up images from the repository no more(save images in its 'assets' folder), due to the GitHub Pages size limitation.
-> TODO : Change the 'data-responsive' part, so that it can load up image of different sizes(of which is not necessarily distinguishable from its URL, unlike file path) from CDN properly.