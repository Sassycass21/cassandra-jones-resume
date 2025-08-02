## Colors

- Sky Blue, Header & Footer: #cce5ff
- Soft Gray, Section Backgrounds - Mobile: #f9f9f9
- Misty Blue, Section Backgrounds - 576px+: #e8f4ff
- Deep Blue, Links: #0077cc
- Crimson Red, Breaking News Headline: #ff0000  
- True White, Body Background: #ffffff
- Charcoal Gray, Body Text: #333333
- Light Gray, Section Borders: #dddddd

## Fonts

Header Font: System default
Body Font: System default

## Breakpoints Summary
/* Breakpoint 1: 576px */
@media (min-width: 576px) {
  .story-img {
    max-width: 80%;
    margin: 0 auto 15px auto;
    display: block;
  }

  section {
    background-color: #e8f4ff;
  }
}

/*  Breakpoint 2: 720px */
@media (min-width: 720px) {
  .story-img {
    float: left;
    width: 200px;
    margin-right: 15px;
  }

  section p {
    overflow: auto;
  }
}

/* Breakpoint 3: 992px */
@media (min-width: 992px) {
  nav ul {
    display: flex;
    justify-content: center;
    gap: 40px;
  }

  nav li {
    display: inline-block;
    margin: 0;
  }

  #breaking-news {
    display: block;
    margin-top: 10px;
  }
}