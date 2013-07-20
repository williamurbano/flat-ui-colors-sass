# Easy to Remember Flat-UI colors.

## What is this?
A set of easy to remember sass variables referencing colors from
[Flat UI](http://designmodo.github.io/Flat-UI/).

## How does it work?

Colors are divided into 7 named groups:
  * **blue**        (4 shades)
  * **gray**        (4 shades)
  * **green**       (4 shades)
  * **orange**      (3 shades)
  * **purple**      (2 shades)
  * **red**         (2 shades)
  * **yellow**      (1 shade)

Every Flat-UI color is aliased by a Sass variable like so:
**"$flat-{group name}-{number}"**
where ```{group name}``` is one of the color groups above, and ```{number}```
is a number between 1-4 (1 being the lightest shade in that group).

Thus, since ```purple``` has two shades, it also has two variables:
```$flat-purple-1```, and ```$flat-purple-2```.

### Example - Lightest shade of gray
```sass
  #myDiv {
    color: $flat-gray-1; // clouds
  }
```
### Example - Darkest shade of blue
```sass
  #myDiv {
    color: $flat-blue-4; // midnight blue
  }
```
### Example - Only shade of yellow.
```sass
  #myDiv {
    color: $flat-yellow-1; // sun flower
  }
```

## Install
Clone the repo:
```sh
 git clone git@github.com:obibring/flat-ui-colors-sass.git
```

Copy ```_flat_colors.scss``` into your sass directory:
```sh
  cp flat-ui-colors-sass/_flat_colors <some directory in your sass include path>
```

Import the file at the top of your stylesheet:
```sass
  @import "flat_colors";
```
