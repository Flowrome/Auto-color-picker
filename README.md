# Project Title

AUTO CONTRAST COLOR PICKER

## Getting Started

Hi, this SCSS library will let you to forget about the problems of contrast between background and text.
The file

```
_color-chooser.scss
```

contains a mixin and a function to pick automatically the font color from a background, adjusting the opacity to give a better contrast mix between background and text.

### Prerequisites

There is only one thing you should have to use this library:

```
[SCSS Compiler](https://sass-lang.com/install)
```

### Installing

Just download the file: 

```
_color-chooser.scss
```

Put it in your style folder and import in your index.scss

## Usage

**If you're using the function just call:**

```
choose-contrast(#xxxxxx, true/false [default is false])
```

and associate it to the attribute you want:

```
.class {
    background-color: #000000;
    color: choose-contrast(#000000);
}
-->
.class {
    background-color: #000000;
    color: #ffffff
}
```

**If you are using the mixin use:**

```
@include choose-contrast-color(#xxxxxx, true/false [default is false])
```

include it the class you want:

```
.class {
    background-color: #000000;
    @include choose-contrast-color(#000000);
}
-->
.class {
    background-color: #000000;
    color: #ffffff
}
```

### Examples

See this [Codepen](https://codepen.io/flowrome/pen/vvXbVm).

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [SASS](https://sass-lang.com/) - The CSS library used

## Authors

* **Romeo Nupieri** - [Flowrome](https://github.com/Flowrome)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

