# FAQs

## How to make slideshow stretched full width?

![Slideshow fullwidth](img/faqs/slideshow-fullwidth.jpg) 

Open __Theme Editor__ > __Carousel__ section > check to the option __Allows image to stretch on large screens__:

![Allows images to stretch on large screens](img/faqs/theme-editor-carousel-stretched.jpg)


## How to remove the leaves background image on the first banner of 'Default' style?

![Leaves banner](img/faqs/leaves-banner.jpg)

To remove this leaves image, open __Edit Theme Files__, open file `assets/scss/_theme-custom.scss_`. Add the code below to the end of file:

```css
.emthemesModez-banner--laparis1:first-child .emthemesModez-banner-figcaption {
  background-image: none;
}
```

Save and refresh your homepage to see changes.