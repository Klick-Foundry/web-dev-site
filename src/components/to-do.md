Nav-Floating-1
    *logoSrc
    Why isn't link getting highlighted if I click a button?
Client data
    Check colors, especially dark mode
Footer
    *logoSrc
Other
    *Favicon
    Check Google PageSpeed and delete Why-choose-1662 05 and Stats stat if necessary
<!-- Testimonials page -->
<!-- Gallery page (portfolio) -->

Move original files to assets/ 
Move svg's to src/assets/icons/

Refactor Picture component to use Astro's
Erase all mobileSrc and tabletSrc
Refactor all files with pictures to have a src prop that is ImageMetaData
In every file you define the picture's src, import the image as a component into the src, ex. import Hero from "hero.png"; src={Hero}
    Remember that the image should now be in src/

Use squoosh on images

Edit CsButton1
H1 tags

Read the Pagespeed analysis to figure out what it's saying to do

2. CSS: Render-blocking styles slowing LCP (~120-620ms savings possible) (how do I do this?)
    Ensure you’re using Tailwind JIT mode with strict purging — only styles you use are included.
    Inline critical CSS for above-the-fold content — tools like critical or built-in Astro plugins can help.
    Defer non-critical CSS or split your CSS bundles into critical vs non-critical.
    Use rel="preload" or rel="prefetch" on CSS files where appropriate.
3. JS: Main thread blocking & forced reflows (how do I do this?)
    Audit your JS for forced synchronous layout reads (offsetWidth, getBoundingClientRect inside tight loops or after DOM writes).
    Defer or lazy-load non-critical JS.
    Bundle and minify your JS aggressively.
    Use Astro’s partial hydration or islands approach to reduce client JS.
4. Fonts: Load performance & cache (where do I find this?)
