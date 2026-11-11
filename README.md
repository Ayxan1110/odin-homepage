# Homepage

Project from [The Odin Project – Advanced HTML and CSS](https://www.theodinproject.com/lessons/node-path-advanced-html-and-css-homepage).

**Live demo:** https://ayxan1110.github.io/odin-homepage/

My personal homepage: a short introduction, a "My work" grid with the projects I built in the course (screenshot, description, live demo and GitHub link for each), and a contact section. The layout works from 320px up to 1920px wide. There is no JavaScript, only `index.html` and `style.css`.

## What I used
- **Semantic HTML**: `header`, `nav`, `main`, `section`, `footer`, one `h1`, headings in order, and a "Skip to content" link for keyboard users
- **Natural responsiveness**: the project cards use CSS Grid with `repeat(auto-fit, minmax(min(100%, 280px), 1fr))`, so the grid goes from 1 to 2 to 3 columns without a media query
- **Media queries** (mobile first, `min-width: 640px` and `960px`): bigger spacing on tablets, and on desktop the hero and contact sections become two columns
- **Flexbox** for the header, the nav, the "facts" pills, the buttons and the card content (the links stay at the bottom of every card)
- **Fluid typography** with `clamp()` for the main title, and `min()` for the page width
- **Responsive images**: `srcset` + `sizes` (400px and 800px JPG versions of each screenshot), `width` and `height` attributes so the page does not jump while loading, `loading="lazy"`, and `aspect-ratio` with `object-fit: cover`
- **Custom properties** for all the colours and fonts
- **Transitions and transforms**: cards lift and the screenshot zooms on hover, buttons move up, the logo rotates, the nav underline grows, and the hero fades in with a `@keyframes` animation
- **Accessibility**: alt text on every screenshot, visible `:focus-visible` outlines, `:focus-within` on the cards, links that make sense for screen readers (hidden text such as "Live demo of Library"), good colour contrast, and `prefers-reduced-motion` that turns off every animation and movement
- An inline **SVG** placeholder portrait (basketball with my initials) and inline SVG icons for GitHub and the external link
- Fonts from Google Fonts (Fraunces for headings, Inter for text)

I did not use a stock photo of a person, because I don't have a photo on the page yet. The project screenshots are my own projects.
