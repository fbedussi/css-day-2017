::::slide
:::slide
# Scalable css
by Carla Soloperto

[slide](https://www.slideshare.net/CarlaSoloperto/css-scalabile-sfide-e-ricompense-di-un-percorso-in-salita)
:::

:::slide
## Challenges
- Readable code
- Scalable code
:::

:::slide
## Solutions
- Dry code
- linters
- naming conventions (eg. [corporate CSS/SASS naming convention](https://confluence.nap/display/OFS/CSS+classes+and+SASS+guidelines))
- modular architecture
- code review
:::

:::slide
## Tools
- colornamer (assign a meaningful name to color hex codes)
:::
::::

::::slide
:::slide
# Refactoring CSS
by Mattia Tommasone

[slide](https://speakerdeck.com/raibaz/refactoring-css) - [video](https://vimeo.com/channels/italiancssday/213069524)
:::

:::slide
## When
- Almost always...
- ...but not during the first draft
- when code smells are found
- boy scout rule
- to update a legacy code base to a new standard/library/tool
:::

:::slide
## Code Smells #1 / Undoing

DON'T
````
h2 {
   font-size: 2em;
   margin-bottom: 0.5em;
   padding-bottom: 0.5em;
   border-bottom: 1px solid #ccc;
}
.no-border {
   padding-bottom: 0;
   border-bottom: none;
}
````
:::
:::slide
DO
````
h2 {
   font-size: 2em;
   margin-bottom: 0.5em;
}

.headline {
   padding-bottom: 0.5em;
   border-bottom: 1px solid #ccc;
}
````
:::

:::slide
## Code Smells #2 / Magic numbers
````
height: 37px;
line-height: 1.2em;
width: .7345rem;
border-top: .1875em solid purple;
````
:::

:::slide
## Code Smells #3 / Too much/too less specificity in selectors
````
ul.nav li.active a {}
.content ul.features a.button {}

header {}
h2 {}
````
:::

:::slide
## Code Smells #4 / ID
- unique per page
- overrides any combination of classes
- no need to use them
:::

:::slide
## Tricks
- shame.css
:::
::::

::::slide
:::slide
# CSS performance
by Andrea De Carolis

[slide](https://speakerdeck.com/decarola/le-performance-come-esperienza-religiosa-css-day-2017)
:::

:::slide
A faster site is better than a slower site
- improves SEO
- improves UX
- improves redemption
:::

:::slide
## How to
Images (66% of average page weight)
- responsive images
- lazy load
- image optimisation (MozJpeg, ImageMagick)
:::

:::slide
## Percived vs real performance
 ![](C:\Users\bedussif\Downloads\visual-progress1.png) 
:::

:::slide
- Critical css
- Clean code
- HTTP2
- Mobile first
:::

:::slide
## Goals
- speed index below 1000
- first paint in less than 1 sec
- (when optimising) at least a 20% improvement
:::

:::slide
# How to deal with clients/designers/ecc.?
Performance budget
:::
::::

::::slide
:::slide
# Style guides vs pattern library
by Alessandro Violini

[slide](https://www.slideshare.net/extrategy/dalle-styleguide-alla-pattern-libraries-cosa-serve-e-quando) - [video](https://vimeo.com/channels/italiancssday/213070439)
:::

:::slide
- Style guides vs pattern library
- modularity
- Atomic Design/BEM/OOCSS
:::
::::

::::slide
:::slide
# CSS: figli di un dio minore
by Davide di Pumpo

[slide](https://www.slideshare.net/DavideDiPumpo/css-figli-di-un-dio-minore) - [video](https://vimeo.com/channels/italiancssday/213071094)
:::

:::slide
## Testing CSS
- unit test: es. `expect(el.css('display')).to.be('block')`
- [True](https://github.com/oddbird/true), unit test for Sass
- Regression test
:::
::::

::::slide
:::slide
# The multicolumn challenge: accepted!
by Lorena Ramonda

[slide](https://www.slideshare.net/lorenaramonda/the-multicolumn-challenge-accepted) - [video](https://vimeo.com/channels/italiancssday/213071558)
:::

:::slide
## 6 techniques to get a 3 column layout tested:
1. Table
2. Div display: table
3. Div floated
4. Flexbox
5. CSS Grid
6. CSS Columns
:::

:::slide
## Results: speed
1. Flexbox ~809ms
2. Table ~860ms
3. Div floated ~915ms
4. CSS Grid ~927ms
5. Div display: table ~1030ms
6. CSS Columns ~1448ms
:::

:::slide
## Compatibility
1. Table > ALL
2. Div floated > ALL
3. Div display: table > NO IE 6 & 7
4. Flexbox > NO IE 6-9
5. CSS Columns > NO IE 6-9
6. CSS Grid > NO safari < 10.3 & Android Browser
:::

:::slide
## And the winner is...
Flexbox/CSS Grid
:::
::::

::::slide
# Responsive Images
by Andrea Verlicchi

[slide](http://www.andreaverlicchi.eu/css-day-2017-responsive-images-html-51/)
::::

::::slide
:::slide
# Bootstrap 4 is coming
by Carmine Alfano

[video](https://vimeo.com/channels/italiancssday/213073176)
:::
:::slide
# Improvements
- Sass sources
- Modularity
:::
::::

::::slide
# that's all folks
Francesco Bedussi

francesco.bedussi@ynap.com
::::