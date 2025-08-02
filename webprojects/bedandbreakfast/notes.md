## Colors

- Lodge Green, headers and accents, #355E3B
- Lake Blue, links and buttons, #457b9d
- River Mist, background and sections, #a8dadc
- Wood Taupe, subtle highlights and backgrounds, #e8d4b0
- Snow White, main background, #f8f9fa
- Charcoal Gray, body text, #343A40

## Fonts

Header Font: Playfair Display - Elegant serif, great for names, page titles, and nav.
Body Font: Lato or Open Sans - Clean, easy to read, pairs beautifully with a serif header.

Font Awesome Icon Suggestion:
fa-bed, fa-fire, fa-tree, or fa-envelope


## CSS Positioning
CSS Positioning
Positioning gives you control over where elements appear on the page. Unlike the box model, which controls how elements take up space, positioning lets you shift elements more precisely.

Static
This is the default. Elements follow the normal document flow. No special positioning applied.

Relative
Moves the element relative to where it would normally be. You can shift it up, down, left, or right.
🔸 The space it originally took up stays put — other content won’t move around it.
🔸 It can overlap other elements.

Fixed
Stays in a fixed position in the browser window — even when you scroll.
🔸 Useful for sticky headers or always-visible navigation.
🔸 Positioned relative to the viewport.

Absolute
Moves the element relative to the nearest positioned ancestor (anything that's not static).
🔸 The element is removed from the normal flow — surrounding content fills its old spot.
🔸 Precise control, but requires awareness of its parent’s position.

## Font Awesome
Font Awesome is a library of icons you can easily use in your websites — perfect for adding visual interest or guiding users.

Instead of using image files, you use special HTML tags with class names. This keeps things lightweight and customizable with CSS!

To use Font Awesome:

Add the link to your HTML <head> (or use a CDN):
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

Use an icon with a tag like this:
<i class="fas fa-coffee"></i>
That will show a coffee cup! ☕️
You can style icons just like text:
i {
color: brown;
  font-size: 24px;
}

Explore more icons at: fontawesome.com/icons


/* Z-Index (fix positioning overlapping) */
add z-index to positioning, highest number is top layer