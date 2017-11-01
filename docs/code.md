---
layout: single-col
title: Sample Essay
date: 2017-02-19
---

{% include jumbotron.html
  title="Essay Example"
  image="images/BirdsEye_1886.jpg"
  text="This is where you put your catchy subtitle.
" %}


*This page provides a bogus essay, beginning with a full bleed header image to illustrate how to implement the various typographic features we're using. The gray boxes should show you exactly what code you need to use; copy and paste it into your own essay pages and adjust the attributes as you need to.*

**To use this layout, make sure you have `layout: single-col` in your page header**

In all of the below examples, make sure you take extreme care with your quotation marks and other coding symbols!


To achieve a jumbotron header, use the following code on your page, and alter the image filename and text accordingly:

``` html
{%raw%}{% include jumbotron.html
title="Essay Example"
image="images/BirdsEye_1886.jpg"
text="This is where you put your catchy subtitle."
%} {%endraw%}
```


## Images
There is one basic way we will embed images in our essay files. Note that it is totally different from how you learned to do them in Markdown itself. This is because if we want to maintain consistency between images, like how the captions appear, we have to make sure we display all images exactly the same way.

### Standard Usage

{% include figure.html class="img-right" width="33%" caption="Centennial Hotel" src="images/centennial-hotel.jpg" %}

Fusce vulputate eleifend sapien. Vestibulum purus quam, scelerisque ut, mollis sed, nonummy id, metus. Nullam accumsan lorem in dui. Cras ultricies mi eu turpis hendrerit fringilla. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; In ac dui quis mi consectetuer lacinia. Nam pretium turpis et arcu. Duis arcu tortor, suscipit eget, imperdiet nec, imperdiet iaculis, ipsum.


To embed the image above, we use:
```
{%raw%}{% include figure.html class="img-right" width="33%" caption="Centennial Hotel" src="images/centennial-hotel.jpg" %}{%endraw%}
```


### Use whatever width you want
You can alter the width of the image as a percentage of our standard page width. You can have them appear on the left, right, or center of the page.


{% include figure.html class="img-left" width="50%" src="/images/centennial-hotel.jpg" caption="Obviously we need a 50% image somewhere."%}

Fusce vulputate eleifend sapien. Vestibulum purus quam, scelerisque ut, mollis sed, nonummy id, metus. Nullam accumsan lorem in dui. Cras ultricies mi eu turpis hendrerit fringilla.

Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; In ac dui quis mi consectetuer lacinia. Nam pretium turpis et arcu. Duis arcu tortor, suscipit eget, imperdiet nec, imperdiet iaculis, ipsum.


To achieve the above half-width image, use:
```
{%raw%}{% include figure.html
class="img-left"
width="50%"
src="images/centennial-hotel.jpg"
%}{%endraw%}
```


Fusce vulputate eleifend sapien. Vestibulum purus quam, scelerisque ut, mollis sed, nonummy id, metus. Nullam accumsan lorem in dui. Cras ultricies mi eu turpis hendrerit fringilla. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; In ac dui quis mi consectetuer lacinia. Nam pretium turpis et arcu. Duis arcu tortor, suscipit eget, imperdiet nec, imperdiet iaculis, ipsum.

{% include figure.html class="img-center" width="100%" caption="Centennial Hotel" src="images/centennial-hotel.jpg" %}

To achieve the above full-width (but not jumbotron) image, use:
{%raw%}
```
{% include figure.html class="img-center" width="100%" caption="Centennial Hotel" src="images/centennial-hotel.jpg" %}
```
{%endraw%}


### Juxtapose
It's easy to set up a slider to compare historic and contemporary photos. If you find a historic image from a vantage point that you can replicate, please take a modern photo so we can better illustrate the changes in the surrounding space.

{% include juxtapose.html
image1="/images/kimo-1928.jpg"
image2="/images/kimo-1938.jpg"
%}

```
{%raw%}{% include juxtapose.html
image1="/images/kimo-1928.jpg"
image2="/images/kimo-1938.jpg"
%}{%endraw%}
```




## Pull Quotes

As part of our effort to highlight our most important ideas---even in the context of relatively short essays---we want to use pull quotes.

### Standard usage
{% include aside.html class="pullquote" text="
Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Fusce id purus. Ut varius tincidunt libero. Phasellus dolor. Maecenas vestibulum mollis diam. Pellentesque ut neque." %}

Aenean vulputate eleifend tellus. Aenean leo ligula, porttitor eu, consequat vitae, eleifend ac, enim. Aliquam lorem ante, dapibus in, viverra quis, feugiat a, tellus. Phasellus viverra nulla ut metus varius laoreet. Quisque rutrum. Aenean imperdiet. Etiam ultricies nisi vel augue. Curabitur ullamcorper ultricies nisi. Nam eget dui. Etiam rhoncus.


To place a pull quote as above, we use:


```
{%raw%}{% include aside.html class="pullquote" text="
Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Fusce id purus. Ut varius tincidunt libero. Phasellus dolor. Maecenas vestibulum mollis diam. Pellentesque ut neque." %}{%endraw%}
```

### Full-width usage
If you are quoting from a historical source, you might want to say more than can fit in a normal pull quote format. For those cases, you can use a full-width blackquote to highlight a particularly juice quotation.

{% include full-width.html class="pullquote" text="
Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Fusce id purus. Ut varius tincidunt libero. Phasellus dolor. Maecenas vestibulum mollis diam. Pellentesque ut neque.
" %}

To achieve the above full width pull quote, use:

```
{%raw%}{% include full-width.html class="pullquote" text=" Vestibulum ante ipsum primis in faucibus orci luctus ..." %}{%endraw%}
```
