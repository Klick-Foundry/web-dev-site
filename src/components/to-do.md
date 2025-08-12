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
Make universal assets file

Refactor Picture component to use Astro's
Erase all mobileSrc and tabletSrc
Refactor all files with pictures to have a src prop that is ImageMetaData
In every file you define the picture's src, import the image as a component into the src, ex. import Hero from "hero.png"; src={Hero}
    Remember that the image should now be in src/

Use squoosh on images

Edit CsButton1
H1 tags

Nav component styles is:inline
